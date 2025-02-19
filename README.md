# Théorèmes et Séries en Analyse Mathématique

Ce document présente plusieurs théorèmes et concepts liés à l'intégration, aux séries de fonctions, aux séries entières et aux séries de Fourier.

## 1. Théorèmes d'Intégration

### Théorème de Convergence Monotone
Soit \( (f_n)_{n\geq 0} \) une suite croissante de fonctions intégrables et positives. Alors :

$$
\lim_{n\to\infty} \int f_n(x)dx = \int \lim_{n\to\infty} f_n(x)dx.
$$

### Théorème de Convergence Dominée
Soit \( (f_n)_{n\geq 0} \) une suite de fonctions intégrables et \( f \) une fonction intégrable telle que :

- \( \lim_{n\to\infty} f_n(x) = f(x) \) presque partout.
- Il existe une fonction intégrable \( \phi \) telle que \( |f_n(x)| \leq \phi(x) \).

Alors :

$$
\lim_{n\to\infty} \int f_n(x)dx = \int f(x)dx.
$$

## 2. Séries de Fonctions

### Convergence Simple
Une série de fonctions \( \sum f_n(x) \) converge simplement sur \( J \) si :

$$
\lim_{n\to\infty} S_n(x) = \sum_{n=0}^{\infty} f_n(x)
$$

pour tout \( x \in J \).

### Convergence Uniforme
Une série de fonctions \( \sum f_n(x) \) converge uniformément sur \( J \) si :

$$
\sup_{x\in J} |S_n(x) - S(x)| \to 0 \quad \text{quand } n \to \infty.
$$

### Critère de Weierstrass
Si il existe une série numérique \( \sum a_n \) convergente telle que :

$$
\forall x \in J, \forall n \in \mathbb{N}, |f_n(x)| \leq a_n,
$$

alors la série \( \sum f_n(x) \) converge uniformément.

## 3. Séries Entières

### Rayon de Convergence
Une série entière s’écrit sous la forme :

$$
\sum a_n z^n.
$$

Son rayon de convergence est donné par :

$$
R = \frac{1}{\limsup_{n\to\infty} \sqrt[n]{|a_n|}}.
$$

### Dérivation et Intégration des Séries Entières
Si \( \sum a_n z^n \) a un rayon de convergence \( R \), alors on peut la dériver terme à terme :

$$
\left( \sum a_n z^n \right)' = \sum n a_n z^{n-1}.
$$

De même, sa primitive est donnée par :

$$
\int \sum a_n z^n dz = \sum \frac{a_n}{n+1} z^{n+1}.
$$

## 4. Séries de Fourier

### Définition
Une série de Fourier associée à une fonction \( f \) est donnée par :

$$
\frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos(nx) + b_n \sin(nx) \right]
$$

avec les coefficients :

$$
a_n = \frac{1}{\pi} \int_{0}^{2\pi} f(x) \cos(nx) dx, \quad
b_n = \frac{1}{\pi} \int_{0}^{2\pi} f(x) \sin(nx) dx.
$$

### Théorème de Dirichlet
Si \( f \) est une fonction périodique vérifiant les conditions de Dirichlet, alors sa série de Fourier converge et :

$$
\sum_{n=1}^{\infty} \left[ a_n \cos(nx) + b_n \sin(nx) \right] \to f(x).
$$

### Égalité de Parseval
Si \( f \) est développable en série de Fourier, alors :

$$
\frac{a_0^2}{2} + \sum_{n=1}^{\infty} (a_n^2 + b_n^2) = \frac{1}{\pi} \int_{0}^{2\pi} f^2(x) dx.
$$

---

**Références :**
- Théorèmes d’intégration
- Séries de fonctions et convergence
- Séries entières et rayon de convergence
- Développement en séries de Fourier
