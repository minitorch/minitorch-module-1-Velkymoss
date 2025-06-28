---

### Given

A function

$$
f: \mathbb{R}^2 \to \mathbb{R}, \quad f(x_1, x_2)
$$

and a **path** (or input constraint)

$$
z(x) = (x, x) \in \mathbb{R}^2,
$$

where both inputs are equal and depend on a **single scalar variable** $x \in \mathbb{R}$.

---

### Goal

Find the derivative of the scalar function

$$
h(x) := f(z(x)) = f(x, x).
$$

---

### By the chain rule for multivariate functions

$$
\frac{dh}{dx} = \nabla f (z(x)) \cdot \frac{dz}{dx}.
$$

Where:

* $\nabla f (z(x)) = \begin{bmatrix} \frac{\partial f}{\partial x_1} \\[6pt] \frac{\partial f}{\partial x_2} \end{bmatrix}$ evaluated at $(x, x)$,
* and

$$
\frac{dz}{dx} = \frac{d}{dx} \begin{bmatrix} x \\ x \end{bmatrix} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}.
$$

---

### Therefore

$$
\frac{dh}{dx} = \begin{bmatrix} \frac{\partial f}{\partial x_1} \\[6pt] \frac{\partial f}{\partial x_2} \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 1 \end{bmatrix} = \frac{\partial f}{\partial x_1} + \frac{\partial f}{\partial x_2}.
$$

---

### Interpretation

* The gradient $\nabla f$ lives in $\mathbb{R}^2$.
* But since the input moves **only along the line** $x_1 = x_2$, the change of $f$ with respect to $x$ is the projection of $\nabla f$ onto the direction $\frac{dz}{dx} = (1,1)$.
* This projection **sums** the partial derivatives, yielding the **total derivative** with respect to $x$.

---