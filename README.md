# 🧮 Variance Reduction Techniques in Option Pricing

This notebook showcases essential **Monte Carlo variance reduction methods** used in pricing European-style options. These techniques are crucial when dealing with simulations, as they significantly **reduce estimator variance**, improving both speed and accuracy.

---

## 🎯 Objectives

- Implement and compare multiple variance reduction techniques.
- Evaluate their efficiency relative to the standard Monte Carlo method.
- Use each technique to estimate the price of a European call option.

---

## 🛠️ Implemented Techniques

### ✅ Antithetic Variates
Generate pairs of negatively correlated paths by inverting Brownian increments. Averaging results from each pair reduces variance.

### ✅ Control Variates
Leverage the known price of a correlated instrument (like the analytical Black-Scholes price) to adjust the Monte Carlo estimator.

### ✅ Importance Sampling
Change the probability distribution of simulated paths to favor rare but significant events, then correct with a likelihood ratio.

---

## 📊 Outputs

- Side-by-side comparison of the **estimated prices**, **standard deviations**, and **confidence intervals**.
- Visualization of the **convergence speed** for each method.
- Illustration of **variance reduction factor** to quantify efficiency.

---

## 💡 Key Takeaways

- Variance reduction is essential to make Monte Carlo pricing methods more **practical in production**.
- Properly applied, these techniques can **reduce simulation cost by orders of magnitude**.
- The choice of method depends on the **payoff function**, **dimensionality**, and **known analytical results**.

---

## 📚 References

- Pages, G. **Introduction to Numerical Probabilities for Finance**

## 👤 Author

👨‍💻 Guillaume Routier  
🎓 MSc Probabilité & Finance – École Polytechnique & Sorbonne Université  
📬 [Contact me on LinkedIn](https://www.linkedin.com/in/guillaume-routier/)

---

## 📌 Disclaimer

These notebooks are for educational and demonstrative purposes only. They do not constitute financial advice.