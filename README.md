# ARDL-Growth-Mauritania  

**Modeling the Drivers of Mauritania’s GDP with an ARDL Framework**

---

## 📑 Overview  
This mini-project replicates the econometric analysis presented in the accompanying PDF report  
*“Modélisation économétrique des dynamiques de croissance en Mauritanie : Une approche ARDL appliquée.”*  
Using a small, clean R workflow, we estimate an AutoRegressive Distributed Lag (ARDL) model that links Mauritania’s real GDP to six macro-variables:  

| Symbol | Variable                                   |
| ------ | -------------------------------------------|
| **CM** | Household consumption                      |
| **CP** | Government consumption                     |
| **FBCF** | Gross fixed-capital formation           |
| **VS** | Changes in inventories                     |
| **IMP** | Imports                                   |
| **EX** | Exports                                   |

The goal is to uncover both short-run and long-run relationships and provide policy-relevant diagnostics (cointegration tests, stability checks, normality, etc.).

---

## 🎯 Key Objectives
1. **Clean & load** a compact macro-panel stored in `data/economic_indicators_mauritania.xlsx`.  
2. **Specify & estimate** individual ARDL(p,q) equations for each demand component.  
3. **Perform**  
   * ADF / PP unit-root tests  
   * Pesaran et al. bounds tests for cointegration  
   * CUSUM / CUSUM-SQ stability diagnostics  
4. **Export** tables and plots directly into a reproducible PDF/HTML report.

## 🔧 Quick-start

1. **Clone the repo**
   ```bash
   git clone https://github.com/<your-handle>/ardl-growth-mauritania.git
   cd ardl-growth-mauritania

