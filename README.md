MethodDkaEn

A program for solving high-degree algebraic equations

MethodDkaEn.html

JavaScript

Supported Operating Systems: Windows 11 Home 24H2, Android 15

MIT License

Prototype Evaluation Version 4.00

Linear equations (1st degree) can be solved in the first year of middle school, Quadratic equations (2nd degree) can be solved in the third year of middle school.

Equations of 3rd degree or higher can be solved using Cardano’s formula, or through numerical analysis methods such as Lagrange’s method or Newton's method.

For equations of 4th degree or higher, except for special cases, numerical analysis is required.

Most ordinary programs require initial values or can only find real-number solutions.

However, this program can determine all solutions (including complex numbers) for high-degree equations (up to the 1000th degree) without requiring initial values.

Download the MethodDkaEn.html file from GitHub to your local OS (Windows 11 or Android device), open it in a browser (Edge or Chrome), and execute the script to solve high-degree algebraic equations or factorize them.

First, enter the highest degree in the text box.

An input box will open; enter the coefficients of the real numbers sequentially from the highest degree.

The coefficients for the entered degree will be displayed.

If a specific degree is missing, enter 0 as its coefficient—this cannot be omitted!

For coefficients of +1, input 1; for -1, input -1.

The number of significant figures for solutions is approximately 15 digits. Even if more digits are displayed, they have no meaning, so please be careful!

This program may yield excellent results if used as an initial value for programs aiming for higher-precision solutions!

The author is not responsible for any issues arising from the use of this program. Use it at your own risk (verify the results yourself before using).

Thank you for reading this help file to the end! I would be honored if this program could be helpful to you.

Finally, I extend my gratitude to the teachers who taught me arithmetic and mathematics, and the authors of numerical analysis books!

Since this software is a prototype evaluation version, it is distributed as free software.

This program was created by converting my Android Java source code into JavaScript with the assistance of Microsoft Edge’s Windows Copilot.

Thank you, Microsoft!





---

There are several typical factors that can cause the DKA method (Durand-Kerner-Aberth method) to fail to converge or to converge poorly. For someone well-versed in numerical analysis like Yoshifumi-san, the following points may be particularly noteworthy:

⚠️ Common Causes of Non-Convergence or Poor Convergence

- **Inappropriate selection of initial values**  
  Since the DKA method is based on the Newton method, convergence becomes difficult if the initial values are not close to the actual roots.  
  Especially when multiple roots (duplicate solutions) exist, having initial values too close together can cause denominators to approach zero, leading to numerical instability.

- **Presence of multiple or closely spaced roots**  
  Because the DKA method simultaneously solves for all roots, closely spaced roots can strongly interact, slowing or even preventing convergence.

- **Extreme values in polynomial coefficients**  
  Large variations in coefficient scaling can lead to inaccurate radius estimation for initial values, thus affecting convergence.

- **Inadequate iteration count or tolerance settings**  
  If the tolerance is too large, it may appear to converge while lacking precision; if too small, an excessive number of iterations may be needed to achieve convergence.

- **Numerical rounding errors and computational precision limits**  
  Especially in complex number calculations, rounding errors tend to accumulate, destabilizing the convergence criteria.

🛠️ Tips for Improvement

- Using Aberth's initial values has been shown to significantly improve convergence behavior.

- When dealing with closely spaced roots, combining with other methods (e.g. Jenkins-Traub algorithm or complex plane subdivision methods) may be helpful.

- Scaling or normalizing the coefficients can improve numerical stability.

---


