# 📘 Fixed Income Securities Project – MSc Quantitative Finance

## 🧩 Part I – Bootstrapping Swap Curves

1. **Bootstrap the OIS discount factor** $D_0(0, T)$ using data from `IR Data.xlsm`.  
   - Plot the OIS discount curve for $T \in [0, 30]$ years.

2. **Bootstrap the LIBOR discount factor** $D(0, T)$ from IRS data provided.  
   - Plot the LIBOR discount curve for $T \in [0, 30]$ years.  
   - Assume the market is collateralized in cash and pays overnight interest on posted collateral.

3. **Calculate the following forward swap rates:**
- 1y × 1y, 1y × 2y, 1y × 3y, 1y × 5y, 1y × 10y
- 5y × 1y, 5y × 2y, 5y × 3y, 5y × 5y, 5y × 10y
- 10y × 1y, 10y × 2y, 10y × 3y, 10y × 5y, 10y × 10y
  
  Use linear interpolation where needed.

---

## ⚙️ Part II – Swaption Calibration

1. **Calibrate the Displaced Diffusion model** to swaption vol data from `IR Data.xlsm`.  
- Provide a table of calibrated **σ** and **β** parameters.

2. **Calibrate the SABR model** to the same data using **β = 0.9**.  
- Document the calibrated parameters:
  - α (alpha)  
  - ρ (rho)  
  - ν (nu)

3. **Price the following swaptions** using both calibrated models:

- Payer Swaptions: 2y × 10y with strikes K = 1% to 8%
- Receiver Swaptions: 8y × 10y with strikes K = 1% to 8%

---

## 📊 Part III – Convexity Correction

1. **Using the SABR model**, value CMS-based swap legs:

- CMS10y received semi-annually over 5 years  
- CMS2y received quarterly over 10 years  

2. **Compare forward swap rates vs CMS rates** for:
- 1y × 1y, 1y × 2y, 1y × 3y, 1y × 5y, 1y × 10y
- 5y × 1y, 5y × 2y, 5y × 3y, 5y × 5y, 5y × 10y
- 10y × 1y, 10y × 2y, 10y × 3y, 10y × 5y, 10y × 10y

- **Discuss the convexity correction**:  
  How does maturity and tenor affect the spread between CMS rates and forward swap rates?

---

## 📈 Part IV – Decompounded Options

1. Payoff at T = 5y

$$
\text{CMS}_{10y}^{1/p} - \frac{0.041}{q}, \quad p = 4, \quad q = 2
$$

- Use static replication to compute PV.

2. Modified payoff (with positive truncation)

$$
\left( \text{CMS}_{10y}^{1/p} - \frac{0.041}{q} \right)^+
$$

- Use static replication to compute PV of this structured option as well.
---

## 👤 Contribution Statement

This project was completed as a group assignment for the Fixed Income Securities course. 
Each team member contributed to a specific section of the project.

I was responsible for **Part III – Convexity Correction**.
- 📓 [Part III – Convexity Correction Notebook](./group%20project/Part_III_Convexity_Correction.ipynb)  
- 📄 [Part III – Convexity Correction Report (PDF)](./group%20project/part3.pdf)

