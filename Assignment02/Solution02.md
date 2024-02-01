# Vector Calculus Assignment 2 Solutions

## General Instructions
The following document contains the solutions to the questions for Assignment 2. Please note that the solutions provided may not be the only possible way to solve the questions. They indicate only one of the many (possibly) valid solutions. The solutions provided are relatively crisp and do not include all the steps that you must have. Your solution should be logical and contain all supporting arguments. Feel free to contact any of the TAs via email in case of any discrepancy you find in the solutions provided.

## Question 1
Note: The convention for the symbol used to represent the angle from the z-axis varies. The solutions here use the convention used in class.


In the cylindrical coordinate system, a point is represented in terms of $r, \theta,$ and $z$. Consider a point in the cartesian system, $P(x,y,z)$. Equivalently, in the cylindrical system:

$$
\begin{align*}
x &= r\cos \theta \\ 
y &=r\sin \theta, \\
z &=z 
\end{align*}
$$

We need to find the projection $P_1$ of a point $P(x,y,z)$, on the plane $x=0$. Therefore, we have:

$$
\begin{align*}
r\cos \theta &=0 \\
\implies \cos \theta &=0 \\
\implies \theta &= \pm 90\degree
\end{align*}
$$

However, $r$ is radial distance and must be positive. Since $y=r\sin \theta$, if y is positive, and we consider $\theta=-90\degree$, then $r$ will turn out to be negative, which is a contradiction. Similarly, if y is negative, and we consider $\theta=90\degree$, then $r$ will turn out to be negative. Hence, we must consider both cases.
Thus the projection of the point will be:

$$
\begin{align*}
P_1&=(r, \pm 90\degree,z)
\end{align*}
$$

where:

$$
\begin{cases}
        \theta=90\degree & \text{if } y \ge 0\\
        \theta=-90\degree & \text{if } y < 0\\
    \end{cases}
$$

and $\displaystyle r=\frac{y}{\sin \theta}$. We could also simply say that $r=\lvert y \rvert $. 

Now, we need to find the projection $P_2$ of a point $P(x,y,z),$ on the plane $y=0$. 

Therefore, we have:

$$
\begin{align*}
r\sin \theta &=0 \\
\implies \sin \theta &=0 \\
\implies \theta &= 0\degree \ \text{or} \ 180\degree
\end{align*}
$$

We apply similar logic, except for $x=r\cos \theta$ this time around. Thus:

$$
\begin{align*}
P_2&=(r, 0\degree \text{or}\ 180\degree,z)
\end{align*}
$$

where:

$$
\begin{cases}
        \theta=0\degree & \text{if } x \ge 0\\
        \theta=180\degree & \text{if } x < 0\\
    \end{cases}
$$

and $\displaystyle r=\frac{x}{\cos \theta}$. We could also simply say that $r=\lvert x \rvert $

In the spherical coordinate system, a point is represented in terms of $r, \theta,$ and $\phi$. Consider a point in the cartesian system, $P(x,y,z)$. Equivalently, in the spherical system:

$$
\begin{align*}
x&= r \sin \theta \cos \phi \\
y&= r \sin \theta \sin \phi \\
z&= r \cos \theta
\end{align*}
$$

We need to find the projection $P_1$ of a point $P(x,y,z)$, on the plane $x=0$ Therefore, we have:

$$
\begin{align*}
r \sin \theta \cos \phi &= 0 \\
\implies \sin \theta \cos \phi &= 0 \\
\implies \phi &= \pm 90\degree
\end{align*}
$$

(Since if $\theta=0$, then $y=0$ as well). Thus:

$$
\begin{align*}
P_1&=(r , \pm 90\degree,\theta)
\end{align*}
$$

where: 

$$
\begin{cases}
        \phi=90\degree & \text{if } y \ge 0\\
        \phi=-90\degree & \text{if } y < 0\\
    \end{cases}
$$

Since $\sin \theta$ is always positive. Furthermore, $r=\sqrt{y^2+z^2}$ and $\theta=\tan^{-1}\left(\frac{y}{z}\right)$. If $\theta<0$, we set $\theta$ as $(\theta+180\degree)$.

We can solve similarly for $P_2$. We need to find the projection $P_2$ of a point $P(x,y,z)$, on the plane $x=0$. Therefore, we have:

$$
\begin{align*}
r \sin \theta \sin \phi &= 0 \\
\implies \sin \theta \sin \phi &= 0 \\
\implies \phi &= 0\degree \text{or} 180\degree
\end{align*}
$$

Since if $\theta=0$, then $x=0$ as well. Thus:

$$
\begin{align*}
P_2&=(r , 0\degree \ \text{or} \ 180\degree,\theta)
\end{align*}
$$

where: 

$$
\begin{cases}
        \phi=0\degree & \text{if } x \ge 0\\
        \phi=180\degree & \text{if } x < 0\\
    \end{cases}
$$

Since $\sin \theta$ is always positive. Furthermore, $r=\sqrt{x^2+z^2}$ and $\theta=\tan^{-1}\left(\frac{x}{z}\right)$. If $\theta<0$, we set $\theta$ as $(\theta+180\degree)$


## Question 2
We know that the for a spherical coordinate system, i.e., a coordinate system defined by $P(r, \theta, \phi)$

$$
\begin{align*}
x &= r \sin \theta \cos \phi \\
y &= r \sin \theta \sin \phi \\
z &= r \cos \theta
\end{align*}
$$

where $\theta$ is the angle with respect to $z$-axis and $\phi$ is the angle that  the projection of $r$ on the $xy$-plane subtends with $x$-axis.

According to the new coordinate system, $\theta$ is the angle with respect to $y$-axis and $\phi$ is the angle that  the projection of $r$ on the $zx$-plane subtends with $x$-axis. The modified expressions for $x, y$ and $z$ are

$$
\begin{align*}
x &= r \sin \theta \cos \phi \\
y &= r \cos \theta \\
z &= r \sin \theta \sin \phi \\
\end{align*}
$$

Thus any point $P(r, \theta, \phi)$ is given by 

$$
\begin{align*}
r &= \sqrt{x^2 + y^2 + z^2} \\
\theta &= \cos^{-1}\left({y \over \sqrt{x^2 + y^2 + z^2}}\right) \\
\phi &= \tan^{-1}\left({z \over x}\right)
\end{align*}
$$

## Question 3

$a)$ Given $\langle\left(\mathbf{a}\times\mathbf{b}\right), \left(\mathbf{c}\times \mathbf{d}\right)\rangle$ and $\mathbf{a}, \mathbf{b}, \mathbf{c}, \mathbf{d} \in \mathbb{R}^3$

Let $\mathbf{a}\times \mathbf{b} = \mathbf{x}$

$$
\begin{align*}
\implies \langle\left(\mathbf{a}\times\mathbf{b}\right), \left(\mathbf{c}\times \mathbf{d}\right)\rangle &= \langle \mathbf{x}, \mathbf{c} \times \mathbf{d}\rangle \\
&= \langle \mathbf{c},\mathbf{d}\times \mathbf{x}\rangle \\
&= \langle \mathbf{c}, \mathbf{d} \times \left(\mathbf{a} \times \mathbf{b}\right)\rangle\\
&= \langle \mathbf{c}, \langle\mathbf{d},\mathbf{b}\rangle\mathbf{a} - \langle\mathbf{d},\mathbf{a}\rangle\mathbf{b}\rangle\\
&= \langle \mathbf{d},\mathbf{b}\rangle\langle \mathbf{a},\mathbf{c}\rangle - \langle \mathbf{d},\mathbf{a}\rangle\langle \mathbf{b},\mathbf{c}\rangle\\
&= \langle\mathbf{a},\mathbf{c}\rangle\langle\mathbf{b},\mathbf{d}\rangle - \langle\mathbf{a},\mathbf{d}\rangle\langle\mathbf{b},\mathbf{c}\rangle
\end{align*}
$$

The second equality is true because of the fact that in scalar triple product $\langle \mathbf{a},\mathbf{b}\times \mathbf{c}\rangle = \langle \mathbf{b},\mathbf{c}\times \mathbf{a}\rangle = \langle \mathbf{c},\mathbf{a}\times \mathbf{b}\rangle$.

<p align='right'>$\square$</p>

$b)$ Given $\left(\mathbf{a}\times\mathbf{b}\right)\times \left(\mathbf{c}\times \mathbf{d}\right)$. 

Let $\mathbf{a}\times \mathbf{b} = \mathbf{x}$

$$
\begin{align*}
\implies \left(\mathbf{a}\times\mathbf{b}\right)\times \left(\mathbf{c}\times \mathbf{d}\right) &= \mathbf{x}\times \left(\mathbf{c}\times \mathbf{d}\right)\\
&=\langle\mathbf{x},\mathbf{d}\rangle\mathbf{c} - \langle\mathbf{x},\mathbf{c}\rangle\mathbf{d}\\
&=\langle\mathbf{a}\times \mathbf{b},\mathbf{d}\rangle\mathbf{c} - \langle\mathbf{a}\times \mathbf{b},\mathbf{c}\rangle\mathbf{d}\\
\implies \left(\mathbf{a}\times\mathbf{b}\right)\times \left(\mathbf{c}\times \mathbf{d}\right) &=\left[\langle\mathbf{a}\times \mathbf{b},\mathbf{d}\rangle\right]\mathbf{c} - \left[\langle\mathbf{a}\times \mathbf{b},\mathbf{c}\rangle\right]\mathbf{d}
\end{align*}
$$

<p align='right'>$\square$</p>

## Question 4
2 Dimensional spherical coordinates are nothing but circular coordinates i.e. 

$$
\begin{align*}
x &= r\cos\theta \\
y &= r\sin\theta
\end{align*}
$$

So, the equation of line $y = mx + c$ can be written as

$$
\begin{align*}
r\sin\theta &= mr\cos\theta + c \\
\implies r &= \frac{c}{\sin\theta - m\cos\theta}
\end{align*}
$$

If we consider the 3D spherical coordinates which are 

$$
\begin{align*}
x &= r\sin\theta\cos\phi \\
y &= r\sin\theta\sin\phi \\
z &= r\cos\theta
\end{align*}
$$

then, the equation $y = mx + c$ is not an equation of line but an equation of plane, so we would need to assume that $z=k$ where $k$ is some random constant is also given. So, the equation of line would become

$$
\begin{align*}
r\sin\theta\sin\phi &= mr\sin\theta\cos\phi + c \\
\implies r &= \frac{c}{\sin\theta\sin\phi - m\sin\theta\cos\phi} \\
\implies r &= \frac{c}{\sin\theta(\sin\phi - m\cos\phi)} \\
\implies r\cos\theta &= \frac{c\cos\theta}{\sin\theta(\sin\phi - m\cos\phi)} \\
\implies r\cos\theta &= \frac{c\cot\theta}{\sin \phi - m\cos\phi} \\
\end{align*}
$$

Using the fact that $r\cos\theta = z = k$, we get

$$
\begin{align*}
&\frac{c\cot\theta}{\sin \phi - m\cos\phi} = k \\
\implies& \cot\theta = \frac{k}{c}(\sin \phi - m\cos\phi) \\
\implies& \theta = \cot^{-1}\left(\frac{k}{c}(\sin \phi - m\cos\phi)\right)
\end{align*}
$$

Similarly, the equation of the plane $ax + by + cz + d = 0$ in the 3D spherical coordinates would be

$$
\begin{align*}
ar\sin\theta\cos\phi + br\sin\theta\sin\phi + cr\cos\theta + d &= 0 \\
\end{align*}
$$

## Question 5
Using the equation of the plane found in the preivous question we can write 

$$
\begin{align*}
ar\sin\theta\cos\phi + br\sin\theta\sin\phi + cr\cos\theta + d &= 0 \\
\end{align*}
$$

Considering some $\phi = \phi_0$ which fixes the plane in 3D dimensional space. Now, allow $\theta$ to vary freely. This gives the family of lines lying on the plane described above. This is the only constraint that you need to impose in order to convert the given plane to a line. 

For example, consider the case: $\phi = 90\degree$; this fixes the plane as the $xy$ plane on varying $\theta$ and $r$ freely. This gives the family of lines lying on the $xy$ plane. 
