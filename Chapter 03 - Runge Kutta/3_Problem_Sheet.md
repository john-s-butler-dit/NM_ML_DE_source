<!-- #region -->
# Problem Sheet 3 - Runge Kutta
1. a) Apply the Midpoint Method to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution:
\begin{equation} y'=t-y, \ \ (0\leq t \leq 4),\end{equation}
with the initial condition $y(0)=1,$
Let $N=4$,  with the exact solution
\begin{equation}y(t)=2e^{-t}+t-1.\end{equation}


1. b) Apply the Midpoint Method to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution:
\begin{equation}y'=y-t, \ \ (0\leq t \leq 2),\end{equation}
with the initial condition $y(0)=2,$
Let $N=4$, with the exact solution
\begin{equation}y(t)=e^{t}+t+1.\end{equation}



2. a) Apply the 4th Order Runge Kutta Method to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution
\begin{equation}y'=t-y, \ \ (0\leq t \leq 4),\end{equation}
with the initial condition $y(0)=1,$
Let $N=4$, with the exact solution
\begin{equation}y(t)=2e^{-t}+t-1.\end{equation}


2. b) Apply the 4th Order Runge Kutta Method to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution
\begin{equation}y'=y-t, \ \ (0\leq t \leq 2)\end{equation}
with the initial condition $y(0)=2,$
$N=4$, with the exact solution
\begin{equation}y(t)=e^{t}+t+1.\end{equation}



3. Derive the difference equation for the Midpoint Runge Kutta method
\begin{equation} w_{n+1}=w_n+k_2,\end{equation}
\begin{equation}k_1=hf(t_n,w_n),\end{equation}
\begin{equation}k_2=hf(t_n+\frac{1}{2}h,w_n+\frac{1}{2}k_1),\end{equation}
for solving the ordinary differential equation
\begin{equation} \frac{dy}{dt}=f(t,y), \end{equation}
\begin{equation}y(t_0)=y_0, $$
by using a formula of the form
\begin{equation} w_{n+1}=w_n+ak_1+bk_2, \end{equation}
where $k_1$ is defined as above,
\begin{equation}k_2=hf(t_n+\alpha h,w_n+\beta k_1),\end{equation}
and $a$, $b$, $\alpha$ and $\beta$ are constants are determined. Prove that $a+b=1$ and $b\alpha=b\beta=\frac{1}{2}$ and choose appropriate values to give the Midpoint Runge Kutta method.


<!-- #endregion -->
```python

```
