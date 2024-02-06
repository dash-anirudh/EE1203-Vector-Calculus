# Question 1

$$
\begin{align*}
f(x,y,z)=e^xcos(yz)
\end{align*}
$$
$$
\begin{align*} 
v&= 2\hat{x}+\hat{y} -2\hat{z} \\
\end{align*}
$$
$$
\begin{align*}
\implies \lVert v \rVert&= 3\\
\end{align*}
$$
$$
\begin{align*}
\implies \hat{v}=\frac{2}{3}\hat{x}+\frac{1}{3}\hat{y}-\frac{2}{3}\hat{z}\\
\end{align*}
$$
$$
\begin{align*}
\implies \hat{v}=a\hat{x}+b\hat{y}-c\hat{z}\\
\end{align*}
$$
$$
\begin{align*}
D_v(f(x,y,z ))&=f_x(x,y,z)a+f_y(x,y,z)b+f_z(x,y,z)c
\end{align*}
$$
$$
\begin{align*}
f_x(x,y,z)&= e^xcos(yz) \\
f_y(x,y,z)&= -ze^xsin(yz) \\
f_y(x,y,z)&= -ye^xsin(yz) \\
\end{align*}
$$
$$
\begin{align*}
\implies D_v(f(x,y,z ))&= \frac{2}{3}e^xcos(yz)+\frac{1}{3}-ze^xsin(yz)-\frac{2}{3}-ye^xsin(yz)\\
\end{align*}
$$

# Question 5
**a)** We need to evaluate a cascade of cross products here. We will solve the inner one first, followed by the outer one.
$$
\begin{align*}
g&= x^2y\hat{x} -2xz\hat{y} + 2yz\hat{z}
\end{align*}
$$
$$
\begin{align*}
\nabla \times g&= \begin{bmatrix}
\mathbf{\hat{x}} & \mathbf{\hat{y}} & \mathbf{\hat{z}}\\ 
\frac{\partial }{\partial x} & \frac{\partial }{\partial y} & \frac{\partial }{\partial z} \\
x^2y & -2xz & 2yz
\end{bmatrix} \\
&= (2x+2z)\hat{x}-(x^2+2z)\hat{z}
\end{align*}
$$
$$
\begin{align*}
\implies \nabla \times 
\begin{bmatrix}
\mathbf{\hat{x}} & \mathbf{\hat{y}} & \mathbf{\hat{z}}\\ 
\frac{\partial }{\partial x} & \frac{\partial }{\partial y} & \frac{\partial }{\partial z} \\
x^2y & -2xz & 2yz 
\end{bmatrix} \\ 
\end{align*}
$$

$$
\begin{align*}
&= \nabla \times [(2x+2z)\hat{x}-(x^2+2z)\hat{z}] \\
&= \begin{bmatrix}
\mathbf{\hat{x}} & \mathbf{\hat{y}} & \mathbf{\hat{z}}\\ 
\frac{\partial }{\partial x} & \frac{\partial }{\partial y} & \frac{\partial }{\partial z} \\
(2x+2z) & 0 & -(x^2+2z)  
\end{bmatrix} \\ 
\end{align*}
$$
$$
\begin{align*}
= 2(x+1)\hat{y}
\end{align*}
$$

**b)** Let's solve this for a general case:

$$
\begin{align*}
\nabla \cdot (\nabla \times g) &= \nabla \cdot 
\begin{bmatrix}
\mathbf{\hat{x}} & \mathbf{\hat{y}} & \mathbf{\hat{z}}\\ 
\frac{\partial }{\partial x} & \frac{\partial }{\partial y} & \frac{\partial }{\partial z} \\
g_x & g_y & g_z  
\end{bmatrix} \\ 
\end{align*}
$$
$$
\begin{align*}
= \nabla \cdot \left[\left(\frac{\partial g_z}{\partial y}-\frac{\partial g_y}{\partial z}\right)\hat{x}+\left(\frac{\partial g_x}{\partial z}-\frac{\partial g_z}{\partial x}\right)\hat{y}+\left(\frac{\partial g_y}{\partial x}-\frac{\partial g_x}{\partial y}\right)\hat{z}\right]
\end{align*}
$$
$$
\begin{align*}
= \frac{\partial}{\partial x}\left(\frac{\partial g_z}{\partial y}-\frac{\partial g_y}{\partial z}\right)+\frac{\partial}{\partial y}\left(\frac{\partial g_x}{\partial z}-\frac{\partial g_z}{\partial x}\right)+\frac{\partial}{\partial z}\left(\frac{\partial g_y}{\partial x}-\frac{\partial g_x}{\partial y}\right) \\
\end{align*} \\
= 0
$$

Thus, irrespective of the function, as long as its second partial derivatives are continuous, the answer is 0. 
