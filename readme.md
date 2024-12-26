This project was developed as part of the Linear Algebra and Optimization for Machine Learning class. The aim is to approximate the solution of the following boundary value problem using different types of feedforward neural networks.  

$-\Delta u = 2\pi^2\sin(\pi x)\sin(\pi y) \quad$   in $\Omega = [0,1]^2$

$u = b \quad$ on $\partial \Omega$

The exact analytical solution is given by $u(x,y) = a\sin(\pi x)\sin(\pi y) + b$.

First, a simple feedforward neural network class is implemented and trained on the problem with $a = 1$ and $b=1$. Then, the [DeepONet](https://arxiv.org/abs/1910.03193) architucture is used to approximate the solution, varying $a$ and $b$ as well in $[-1,1]$.
