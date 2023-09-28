# Problem Sheet 6 - Systems of Equations and Boundary Value Problems


## Question 1

1. Apply the Euler method to estimate the solution of the system of equations
\begin{align} \frac{dx}{dt}= x-0.2xy; &\ \ x(1) = 10;\\
\frac{dy}{dt}= y + 0.1xy; &\ \  y(1) = 2;
\end{align}
using a stepsize h = 0.25, giving the approximate value of the solution at t = 2.0.


## Question 2

2. Use the  Euler method to estimate the solution of the Lorenz system of first order initial value problems, 
\begin{align} \frac{dx}{dt}=\sigma(y-x),& \ \ \ x(0)=1,\\
 \frac{dy}{dt}=x(\rho-z)-y, &\ \ \ y(0)=1,\\
 \frac{dz}{dt}=xy-\beta z,& \ \ \ z(0)=1,\end{align}
 
where $\sigma=8$, $\rho=2$ and $\beta=\frac{7}{3}$,  and
using $h=0.25$, estimate the value of the solution at $t=1.0$.


## Question 3

3. 	Consider the boundary value problem 
\begin{equation} y''=3xy'-4y+x^2, \ \ 1\leq x \leq 2, \ \ y(1)=2,\ \ \ y(2)=-1.\end{equation} 
Apply the linear shooting method to transform this equation into two second order initial value problems
and approximate the solution using the Euler method with stepsize $h=\frac{1}{3}.$

## Question 4

4. Describe in your own words how the linear shooting method is used to numerically approximate a boundary value problem as a system of initial value problems.

## Question 5
5. The Van der Pol oscillator is a non-conservative oscillator with non-linear damping is described by the differential non-linear second order differential equation,
\begin{equation} u^{''}=-\epsilon(u^2-1)u^{'}-u.\end{equation}

Let $\epsilon=1.5$, and given the initial condition
\begin{equation} u(0)=0.0, \text{ and, } u(1)=0. \end{equation}
Apply the one iteration of the non-linear shooting method to approximate the solution from, $0\leq t \leq 1,$ using a stepsize of $h=0.2.$

## Question 6

6. a. Describe in your own words how the non-linear shooting method is used to numerically approximate a boundary value problem as a system of initial value problems.


## Question 7

7. Consider the boundary value problem 
\begin{equation} y''=3xy'-4y+x^2, \ \ 1\leq x \leq 2, \ \ y(1)=2,\ \ \ y(2)=-1.\end{equation} 
Apply the finite difference method to approximate the solution using the Euler method with stepsize $h=\frac{1}{3}.$


