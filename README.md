# ENGR101_MD
# Math Equations Cheat Sheet for GitHub Markdown

## Basics

- **Inline Equations:** Wrap your equation with single dollar signs for inline display. Example: `$E=mc^2$` renders as \(E=mc^2\).

- **Block Equations:** Use double dollar signs for equations that should appear on their own line (block). Example:
renders as 
$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

## Common Symbols and Operations

- **Greek Letters:** Use backslash followed by the letter name. Example: `\alpha`, `\beta`, `\Sigma` for \(\alpha\), \(\beta\), \(\Sigma\).

- **Superscript and Subscript:** Use `^` for superscript and `_` for subscript. Example: `x_i^2` renders as \(x_i^2\).

- **Fractions:** Use `\frac{numerator}{denominator}`. Example: `\frac{a}{b}` renders as \(\frac{a}{b}\).

- **Square Roots:** Use `\sqrt{expression}`. Example: `\sqrt{x^2 + y^2}` renders as \(\sqrt{x^2 + y^2}\).

- **Summations:** Use `\sum` with subscript and superscript for limits. Example: `\sum_{n=1}^{10} n^2` renders as \(\sum_{n=1}^{10} n^2\).

- **Integrals:** Use `\int` with limits for definite integrals. Example: `\int_{0}^{1} x^2 dx` renders as \(\int_{0}^{1} x^2 dx\).

## Advanced Notations

- **Matrices:** Use `\begin{matrix} ... \end{matrix}` for matrices without brackets. Enclose in `\left[` and `\right]` for square brackets:
renders as 
$$\left[
\begin{matrix}
a & b \\
c & d \\
\end{matrix}
\right]$$

- **Equation Arrays:** For aligning equations, use `\begin{align} ... \end{align}`. Ensure you double escape (`\\`) for new lines and `&` for alignment points.

## Tips

- **Escape Special Characters:** Use a backslash (`\`) to escape special Markdown characters when necessary.

- **Experiment:** Try different combinations in a GitHub repository to see how they render and fine-tune your equations.

This cheat sheet covers the basics and some advanced topics for writing math in GitHub Markdown. Experimentation and practice are key to mastering the formatting of complex equations.

