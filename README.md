# MethodDkaEn (200th-degree Polynomial Solver & Factorization Web App)

*MethodDkaEn* is a lightweight, ultra-fast, and high-precision web application designed for solving complex polynomials and performing factorization using pure HTML and JavaScript.

Powered by the **Durand-Kerner (DKA) method**, it combines **50-digit high-precision arithmetic** via `Decimal.js`, **auto-scaling normalization for up to 200th-degree polynomials**, and a convenient **bulk coefficient pasting feature** into a single, seamless web interface.

---

## 🌐 Official Links

* 🚀 **Live Web Application:** [https://YoshiakiKoizumija142397.github.io/MethodDkaEn/](https://YoshiakiKoizumija142397.github.io/MethodDkaEn/)
* 📦 **GitHub Repository:** [https://github.com/YoshiakiKoizumija142397/MethodDkaEn](https://github.com/YoshiakiKoizumija142397/MethodDkaEn)

---

## 📝 Key Features

1. **📋 Bulk Coefficient Input**
   * Easily paste space, line-break, or comma-separated values (e.g., `1 -55 1320 -18150 ...`) to populate all coefficient fields in a single click.

2. **⚡ Auto-Scaling Normalization (Up to Degree 200)**
   * Prevents numerical overflow and underflow even when handling extremely large or tiny coefficients, enabling stable computation across high-degree polynomials.

3. **🎯 50-Digit Precision & Instant Mode Switching**
   * Effortlessly toggle between "50-Digit High-Precision Roots" and "Factored Form" (rounded for readability) without re-calculating.

4. **🌐 Offline & Cross-Platform Support**
   * Runs locally in any modern browser (Chrome, Edge, Safari, Firefox, etc.) across Windows, Mac, Linux, iOS, Android, and ChromeOS without requiring backend server resources.

---

## 📁 Repository Structure

```text
MethodDkaEn/
├── index.html             # Main Web Application
└── README.md              # Documentation

```

---

## 🛠️ Usage

1. Select or input the **Degree of Polynomial** ($n \le 200$).
2. Enter coefficients manually or use the **Bulk Input** button to paste multiple coefficients at once.
3. Click **Calculate** to find all real and complex roots with high precision.

```
