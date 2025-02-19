# Math Formulas :

## La dérivée partielle de f par rapport à xk est donnée par :
$$
\frac{\partial f(x_1, x_2, \dots, x_n)}{\partial x_k} = \frac{\partial f(x_1, x_2, \dots, x_n)}{\partial x_k}
$$

La dérivée partielle de \( f(x_1, x_2, \dots, x_n) \) par rapport à \( x_k \) est donnée par :

$$
\frac{\partial f(x_1, x_2, \dots, x_n)}{\partial x_k}
$$

Cela représente la variation de la fonction \( f \) par rapport à la variable \( x_k \) tout en maintenant les autres variables constantes.

### Gradient
Le gradient de \( f(x_1, x_2, \dots, x_n) \) est le vecteur des dérivées partielles de \( f \) par rapport à chacune des variables :

$$
\nabla f(x_1, x_2, \dots, x_n) = \left( \frac{\partial f}{\partial x_1}, \frac{\partial f}{\partial x_2}, \dots, \frac{\partial f}{\partial x_n} \right)
$$

Cela donne la direction de la plus grande augmentation de la fonction.

### Hessienne
La matrice Hessienne est la matrice des dérivées secondes de \( f \) :

$$
H(f) = \begin{pmatrix}
\frac{\partial^2 f}{\partial x_1^2} & \frac{\partial^2 f}{\partial x_1 \partial x_2} & \dots & \frac{\partial^2 f}{\partial x_1 \partial x_n} \\
\frac{\partial^2 f}{\partial x_2 \partial x_1} & \frac{\partial^2 f}{\partial x_2^2} & \dots & \frac{\partial^2 f}{\partial x_2 \partial x_n} \\
\vdots & \vdots & \ddots & \vdots \\
\frac{\partial^2 f}{\partial x_n \partial x_1} & \frac{\partial^2 f}{\partial x_n \partial x_2} & \dots & \frac{\partial^2 f}{\partial x_n^2}
\end{pmatrix}
$$

Cela fournit des informations sur la courbure de la fonction et aide à déterminer si un point est un maximum, un minimum ou un point selle.

### Définition de la Dérivée
La dérivée d'une fonction à un point mesure la variation instantanée de la fonction à ce point. Pour une fonction \( f(x) \), la dérivée est :

$$
f'(x) = \lim_{\Delta x \to 0} \frac{f(x + \Delta x) - f(x)}{\Delta x}
$$

Cela représente la pente de la tangente à la courbe de \( f(x) \) en un point donné.
