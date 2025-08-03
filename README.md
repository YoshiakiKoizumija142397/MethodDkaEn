
### MethodDka  
A program for factoring and solving high-degree algebraic equations  
High-precision version: 50 digits  
Filename: `MethodDkaEn.html`  
Language: JavaScript  
Supported OS: Windows 11 Home 25H2, Android 15  
License: MIT  
Author: Yoshiaki Koizumi  
Email: ja142397@s6.dion.ne.jp  
Prototype evaluation version: 6.00

- First-degree equations are solved by first-year middle school students  
- Second-degree equations by third-year middle school students  
- Third-degree equations or higher can be solved by Cardano’s formula or numerical analysis using Lagrange’s or Newton’s methods  
- Fourth-degree equations and beyond generally require numerical methods unless they are of a special form  

Unlike conventional programs that require initial values or only find real solutions,  
this program finds *all* solutions, including complex roots, for real-coefficient equations up to the 1000th degree — **without any initial values** required.

You can download the `MethodDkaEn.html` file from GitHub onto a Windows 11 or Android device and open it in Edge or Chrome.  
The script will execute, allowing you to factor and solve high-degree algebraic equations.

**How to use:**  
1. Enter the highest degree in the text box  
2. Input the coefficients (real numbers) in descending order of degree  
3. The entered coefficients will be displayed  
Note: Enter 0 for any degrees that do not appear — skipping is not allowed!  
Also, for coefficients of +1 or –1, enter 1 or –1 explicitly.

The number of significant digits for solutions is approximately 50.

**Disclaimer:**  
The author assumes no responsibility for any problems arising from use of this program.  
Use it at your own risk and verify calculations yourself.  
Thank you for reading the help file to the end!  
I’m honored if this program proves useful to you.  
Now upgraded to a fully Japanese-language version.

Finally, I extend gratitude to my mentors who taught me math and arithmetic, and the authors of numerical analysis books that helped shape this work.

As this is a prototype evaluation version, it is distributed as free software.

This program was developed by converting my Java source code (intended for Android) to JavaScript with the help of Microsoft’s Edge Windows Copilot.  
The high-precision 50-digit version was also converted using Windows Copilot.  
Thank you, Microsoft!

---

According to Windows Copilot,  
there are several common factors that cause the DKA method (Durand-Kerner-Aberth) to fail or struggle with convergence — likely of interest to someone with your expertise in numerical analysis

⚠️ **Main Causes of Non-Convergence or Difficulty**
- **Improper initial values:** DKA relies on Newton’s method, and without values close to the roots, convergence is slow or fails  
- **Multiple or closely spaced roots:** These can cause instability or slow convergence due to mutual interaction of simultaneous root calculations  
- **Extreme coefficient values:** Large disparities in scale affect radius estimation and convergence behavior  
- **Inadequate iteration settings:** Loose error tolerance may misrepresent convergence; too tight settings require excessive computation  
- **Rounding errors and precision limits:** Especially with complex numbers, rounding may lead to unstable convergence tests

🛠️ **Tips for Improvement**
- Using Aberth’s initial values improves convergence significantly  
- If roots are very close, hybrid methods like Jenkins-Traub or complex plane subdivision may help  
- Scaling or normalizing coefficients enhances numerical stability

---
