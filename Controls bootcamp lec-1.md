# Lecture 1: Linear Systems

[![hackmd-github-sync-badge](https://hackmd.io/KUWqtygITTyR81yE0Q6iIA/badge)](https://hackmd.io/KUWqtygITTyR81yE0Q6iIA)


###### tags: `Controls Bootcamp`

$$ \dot{x} = Ax + Bu $$
$x \epsilon \mathbb{R}^n$


for this lecture let us consider: 
$$ \dot{x} = Ax $$

The solution is : 
$$ x(t) = e^{At}x(0)$$

## Eigen Values and Eigen Vectors: 

$$a \xi = \lambda \xi $$

$$ T  = [\xi_1, \xi_2 ... \xi_n]$$

$$ D =
  \begin{bmatrix}
    \lambda_{1}  \\
    & \ddots & \\
    & & \lambda_{n}
  \end{bmatrix} $$
  
  
$$AT = TD$$
$$x = Tz$$ z is x in eigen vector system 

$$\dot{x} = T(\dot{z}) = Ax$$

$$T \dot{z} = ATz$$

$$ \therefore \dot{z} = T^{-1}ATz$$

$$\therefore \dot{z} = D z $$


$$ \frac{d}{dt} \begin{bmatrix} 
z_1 \\
z_2  \\
\vdots \\
z_n
\end{bmatrix} =  
  \begin{bmatrix}
    \lambda_{1}  \\
    & \ddots & \\
    & & \lambda_{n}
  \end{bmatrix}
\begin{bmatrix} 
z_1 \\
z_2  \\
\vdots \\
z_n
\end{bmatrix}
 $$


We have: 
$e^{At} = I + At + \frac{A^{2}t^2}{2!} + \frac{A^{3} t^3}{3!} + ...$


but now: 
$e^{TDT^{-1}} = TT^{-1} + TDT^{-1} + TD^2 T^{-1} + ...$

$$    = T[I + D + D^2 + ...]T^{-1}$$

$$ = Te^{Dt} T^{-1}$$
$$\therefore x(t) = Te^{Dt}T^{-1}x(0)$$

