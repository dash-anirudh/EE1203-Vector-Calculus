# Vector Calculus Assignment 4 Solutions

## General Instructions
The following document contains the solutions to the questions for Assignment 4. Please note that the solutions provided may not be the only possible way to solve the questions. They indicate only one of the many (possibly) valid solutions. The solutions provided are relatively crisp and do not include all the steps that you must have. Your solution should be logical and contain all supporting arguments. Feel free to contact any of the TAs via email in case of any discrepancy you find in the solutions provided.

## Question 1
Given 

$$
\begin{align*}
f(x,y) = 3x^2y^2 \hat{x} + 2x^3y \hat{y}
\end{align*}
$$

and 

$$
\begin{align*} 
\mathcal{C} : 2y^3 - x^3 - y^2 - x^2 +2yx^2 - xy^2 - 2y + x + 1 = 0
\end{align*}
$$

Let us define $p = 3x^2y^2$ and $q = 2x^3y$

The given function defines a conservative field as $\displaystyle{{\partial{p} \over \partial{y}} = {\partial{q} \over \partial{x}}} = 6x^2y$. Thus the integral is independent of the path taken and is given by

$$
\begin{align*}
\int_{\mathcal{C}} f \cdot dr = \int_{\mathcal{C}} \nabla F \cdot dr = F(B) - F(A)
\end{align*}
$$

where $A = (-1,0), B = (0.6, 0.8)$ and $F = x^3y^2$.

$$
\begin{align*}
\implies \int_{\mathcal{C}} f \cdot dr = (0.6)^3(0.8)^2 - (-1)^3(0)^2 = 0.13824
\end{align*}
$$

## Question 2
Given the folowing set of lines:

$$
\begin{align*}
y &= {x \over 2}\ \forall \ x\in [0,4] \\
x &= 4 \ \forall \ y\in[-8,2]
\end{align*}
$$

$a)$ The path that will close these lines is simply the line joining the two vertices that are not connected i.e., the line joining $(0,0)$ and $(4,-8)$. 

$$
\begin{align*}
&\implies y-0 = (x-0)\left({{-8-0}\over{4-0}}\right)\\
&\implies y = -2x\\
&\implies y+2x = 0 
\end{align*}
$$

Note that the equation obtained above is the equation of the required line but the region of our concern is $x \in [0,4]$

$b)$ Let the three lines be represented using the three curves $\mathcal{C_1}$, $\mathcal{C_2}$ and $\mathcal{C_3}$ respectively.

$$
\begin{align*}
\mathcal{C_1} &: y = {x \over 2} \;\; \ x\in [0,4] \\
\mathcal{C_2} &: x = 4 \ \;\; \ y\in[2,-8] \\
\mathcal{C_3} &: y = -2x \ \;\; \ x\in[0,4]
\end{align*}
$$

The region enclosed by the three curves is the region enclosed by the lines $y = {x \over 2}$ and $x = 4$ and the line $y = -2x$.

$$
\begin{align*}
\int_\mathcal{C} \left(x^2y^2dx + \left(yx^3+y^2\right)dy\right) &= \int_{\mathcal{C_1}} \left(x^2y^2dx + \left(yx^3+y^2\right)dy\right) + \int_{\mathcal{C_2}} \left(x^2y^2dx + \left(yx^3+y^2\right)dy\right) 
\\\ &  \qquad +\int_{\mathcal{C_3}} \left(x^2y^2dx + \left(yx^3+y^2\right)dy\right)
\end{align*}
$$

Solving each term individually,

$$
\begin{align*}
\int_{\mathcal{C_1}} \left(x^2y^2dx + \left(yx^3+y^2\right)dy\right) &= \int_{0}^{4} \left(x^2\left({x \over 2}\right)^2dx + \left({x \over 2}x^3+\left({x \over 2}\right)^2\right)\left({dx \over 2}\right)\right)\\
&= \int_{0}^{4} \left({x^4 \over 4} + {x^4 \over 4} + {x^2 \over 8}\right)dx\\
&= \int_{0}^{4} \left({x^4 \over 2} + {x^2 \over 8}\right)dx\\
&= \left[{x^5 \over 10} + {x^3 \over 24}\right]_0^4\\
&= {4^5 \over 10} + {4^3 \over 24}\\
\end{align*}
$$


$$
\begin{align*}
\int_{\mathcal{C_2}} \left(x^2y^2dx + \left(yx^3+y^2\right)dy\right) &=\int_{-8}^{2} \left(16y^2dx + \left(64y+y^2\right)dy\right)\\
&=  \int_{-8}^{2} \left(64y+ y^2dy\right)dy\\
&= \left[32y^2 + {y^3 \over 3}\right]_{-8}^2\\
&= 32(2)^2 + {2^3 \over 3} - 32(-8)^2 - {(-8)^3 \over 3}\\
&= 32(4) + {8 \over 3} - 32(64) - {512 \over 3}\\
\end{align*}
$$

$$
\begin{align*}
\int_{\mathcal{C_3}} \left(x^2y^2dx + \left(yx^3+y^2\right)dy\right) &=
\int_{0}^{4} \left(x^2\left(-2x\right)^2dx +\left( \left(-2x\right)x^3+\left(-2x\right)^2\right)(-2) \right) dx\\
&= \int_{0}^{4} \left(4x^4 + 4x^4 - 8x^2\right)dx\\
&= \int_{0}^{4} \left(8x^4 - 8x^2\right)dx\\
&= \left[{8x^5 \over 5} - {8x^3 \over 3}\right]_0^4\\
&= {8 \over 3} (4)^5 - {8 \over 3} (4)^3\\
\end{align*}
$$

$$
\begin{align*}
\int_\mathcal{C} \left(x^2y^2dx + \left(yx^3+y^2\right)dy\right) &= -384
\end{align*}
$$


$c)$ Consider the given integral $\int_\mathcal{C} \left(x^2y^2dx + \left(yx^3+y^2\right)dy\right)$.

Let $\mathbf{g} = x^2y^2\hat{x} + \left(yx^3+y^2\right)\hat{y}, P = x^2y^2$ and $Q = yx^3 + y^2$

As $\mathbf{g}$ is smooth and the region is enclosed by a simple closed curve, the given integral is independent of the path of integration. 

$$
\begin{align*}
\int_\mathcal{C} \left(x^2y^2dx + \left(yx^3+y^2\right)dy\right) &= \oint_\mathcal{C} \mathbf{g} \cdot d\mathbf{r}\\
&= \iint_R \left({\partial Q \over \partial x} - {\partial P \over \partial y}\right)dA
\end{align*}
$$

$$
\begin{align*}
{\partial Q \over \partial x} &= 3yx^2\\
{\partial P \over \partial y} &= 2x^2y\\
\end{align*}
$$

$$
\begin{align*}
\int_\mathcal{C} \left(x^2y^2dx + \left(yx^3+y^2\right)dy\right) &= \iint_R \left(3yx^2 - 2x^2y\right)dA\\
&= \iint_R \left(x^2y(3 - 2)\right)dA\\
&= \iint_R \left(x^2y\right)dA\\
&= \int_{0}^{4} \int_{-2x}^{x/2} \left(x^2y\right)dydx\\
&= \int_{0}^{4} \left[{x^2y^2 \over 2}\right] _ {-2x}^{x/2}dx\\
&= \int_{0}^{4} \left[{x^2 \over 8} - 4x^2\right]dx\\
&= \left[{x^3 \over 24} - {4x^3 \over 3}\right]_0^4\\
&= {4^3 \over 24} - {4^3 \over 3}\\
&= -384
\end{align*}
$$

$d)$ The direction of traversal along the curve $\mathcal{C}$ decides the sign of the integral. If the direction is reversed, the sign of the obtained integral reverses.

## Question 3
The curve given is $y=x^2$. Thus, we can substitute $dy=2xdx$ and $y=x^2$ in the integral, and integrate over $x$ from $-1$ to $2$.

$$
\begin{align*}
    \int_\mathcal{C} (xy \, dx + (x+y) \,dy) \\
\end{align*}
$$

$$
\begin{align*}
 &= \int_{-1}^{2} (x^3 \, dx + (x+x^2)2x \, \ dx) \\
    &= \int_{-1}^{2} 3x^3 \, dx + \int_{-1}^{2} 2x^2 \, dx \\
    &= \left(\frac{3x^4}{4}+\frac{2x^3}{3} \right)\Big|_{-1}^{2} \\
    &= \frac{69}{4}
\end{align*}
$$

## Question 4
Given the vector field $g(x,y,z) = (3x^2 + 6y)\hat x -14yz\hat y +20xz^2 \hat z$, we need to find the line integral along the curve $\mathcal C$ which is a straight line from $(0,0,0)$ to $(1,0,0)$ and then a straight line from $(1,0,0)$ to $(1,1,1)$.

We can split the curve into two parts, $\mathcal C_1$ and $\mathcal C_2$. We can then calculate the line integral over each part and add them up to get the total line integral.

For $\mathcal C_1$, we have $x = t, y = 0, z = 0$ and $dx = dt, dy = 0, dz = 0$. Thus, the line integral over $\mathcal C_1$ is

$$
\begin{align*}
\int_{\mathcal C_1} g \cdot dr &= \int_{0}^{1} (3t^2 + 6\times 0)dt \\
&= \int_{0}^{1} 3t^2 dt \\
&= \left[t^3\right]_0^1 \\
&= 1
\end{align*}
$$

For $\mathcal C_2$, we have $x = 1, y = t, z = t$ and $dx = 0, dy = dt, dz = dt$. Thus, the line integral over $\mathcal C_2$ is

$$
\begin{align*}
\int_{\mathcal C_2} g \cdot dr &= \int_{0}^{1} ((-14t^2) + 20(1)(t^2))dt \\
&= \int_{0}^{1} 6t^2dt \\
&= \left[2t^3\right]_0^1 \\
&= 2
\end{align*}
$$

Thus, the total line integral is $1 + 2 = 3$.

## Question 5
Given 

$$
\begin{align*}
g(x,y) = (2\sin{x})(\cos{(x+y)})(\cos{x})
\end{align*}
$$
and 
$$
\begin{align*} 
\mathcal{C} : x^2 + y^2 = 1
\end{align*}
$$

We analyze the line integral $\int_{\mathcal{C}} (g)\nabla{g} \cdot dr$ by first checking whether $(g)\nabla{g}$ constitutes a conservative field.

We define $p = \displaystyle{g\frac{\partial{g}}{\partial{x}}}$ and $q = \displaystyle{g\frac{\partial{g}}{\partial{y}}}$

$$
\begin{align*} 
\implies \frac{\partial{p}}{\partial{y}} = \frac{\partial{q}}{\partial{x}} = \frac{\partial{g}}{\partial{x}}\frac{\partial{g}}{\partial{y}} + \frac{\partial^2{g}}{\partial{x}\partial{y}}
\end{align*}
$$

Thus $(g)\nabla{g}$ is a conservative function and the line integral of both the clockwise and anti-clockwise traversals along the closed path $\mathcal{C} : x^2 + y^2 = 1$ is $0$.

$$
\begin{align*}
\int_{\mathcal{C}} (g)\nabla{g} \cdot dr = 0
\end{align*}
$$

## Question 6
The given integral is $\int_{\mathcal{C}} g \cdot d\underline{r}$.

The curve $\mathcal{C}$ is defined as follows:

$$
\mathcal{C} = t \cos(\pi t) \hat{x} + t \sin(\pi t) \hat{y} \quad  0 \leq t \leq 1
$$

let $\underline{r} = t \cos(\pi t) \hat{x} + t \sin(\pi t) \hat{y}$

$$
\begin{align*}
g &= e^{xy} \left(2x + x^2y\right) \hat{x} + e^{xy} \left(x^3 + 2y e^{-xy}\right) \hat{y}\\
&= \nabla \left( e^{xy} x^2 + y^2 \right) =: \nabla f(x)
\end{align*}
$$

So, the field $g$ is conservative.

The given integral is independent of the path of integration and depends only on the initial and final points of the curve.

The initial point of the curve is $t = 0$ (say A) and the final point of the curve be B.

$$
r(0) = 0 \hat{x} + 0 \hat{y}\\
f(A = r(0)) = f(0, 0) = 0
$$

$$
\begin{align*}
\int_{\mathcal{C}} g \cdot d\underline{r} &= f(B) - f(A)\\
&= e^{xy} x^2 + y^2 \Bigg|_{t = 1} - 0\\
&= e^{t^2 \sin(\pi t) \cos(\pi t)} t^2 \cos^2(\pi t) + t^2 - t^2 \cos^2(\pi t)\\ 
&= t^2 \left( 1 - \cos^2(\pi t) \left( 1 - e^{t^2 sin(\pi t)\cos(\pi t)}\right) \right)\\
\end{align*}
$$

The maximum value of the integral in the given parametric range is $t = 1$.

$$
\begin{align*}
\int_{\mathcal{C}} g \cdot d\underline{r} &= 1^2 \left( 1 - \cos^2(\pi) \left( 1 - e^{1^2 sin(\pi)\cos(\pi)}\right) \right)\\
&= 1 
\end{align*}
$$
