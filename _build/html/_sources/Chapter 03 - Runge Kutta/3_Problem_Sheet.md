<!-- #region -->
# Problem Sheet 3 - Runge-Kutta

## Question 1

1. 
    a. Apply the Midpoint Method to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution:
    \begin{equation} y'=t-y, \ \ (0\leq t \leq 4),\end{equation}
    with the initial condition $y(0)=1,$
    Let $N=4$,  with the exact solution
    \begin{equation}y(t)=2e^{-t}+t-1.\end{equation}


    b. Apply the Midpoint Method to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution:
    \begin{equation}y'=y-t, \ \ (0\leq t \leq 2),\end{equation}
    with the initial condition $y(0)=2,$
    Let $N=4$, with the exact solution
    \begin{equation}y(t)=e^{t}+t+1.\end{equation}

## Question 2

2. 
    a. Apply the 4th Order Runge-Kutta Method to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution
    \begin{equation}y'=t-y, \ \ (0\leq t \leq 4),\end{equation}
    with the initial condition $y(0)=1,$
    Let $N=4$, with the exact solution
    \begin{equation}y(t)=2e^{-t}+t-1.\end{equation}


    b. Apply the 4th Order Runge-Kutta Method to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution
    \begin{equation}y'=y-t, \ \ (0\leq t \leq 2)\end{equation}
    with the initial condition $y(0)=2,$
    $N=4$, with the exact solution
    \begin{equation}y(t)=e^{t}+t+1.\end{equation}

## Question 3

3. Derive the difference equation for the Midpoint Runge-Kutta method
    \begin{equation} w_{n+1}=w_n+k_2,\end{equation}
    \begin{equation}k_1=hf(t_n,w_n),\end{equation}
    \begin{equation}k_2=hf(t_n+\frac{1}{2}h,w_n+\frac{1}{2}k_1),\end{equation}
    for solving the ordinary differential equation
    \begin{equation} \frac{dy}{dt}=f(t,y), \end{equation}
    with the initial condition
    \begin{equation}y(t_0)=y_0, \end{equation}
    by using a formula of the form
    \begin{equation} w_{n+1}=w_n+ak_1+bk_2, \end{equation}
    where $k_1$ is defined as above,
    \begin{equation}k_2=hf(t_n+\alpha h,w_n+\beta k_1),\end{equation}
    and $a$, $b$, $\alpha$ and $\beta$ are constants are determined. Prove that $a+b=1$ and $b\alpha=b\beta=\frac{1}{2}$ and choose appropriate values to give the Midpoint Runge-Kutta method.

## Question 4

4. For the Runge-Kutta methods describe in your own words the concepts:

    a. Consistency;

    b. Convergence.

## Question 5


5. Describe in your own words the theorem below and its proof:
    Assume that the Runge-Kutta method satisfies the Lipschitz Condition. Then
    for the initial value problems
    \begin{equation} y^{'}=f(x,y),\end{equation}
    \begin{equation} y(x_0)=y_0. \end{equation}
    The numerical solution $\{ w_n\}$ satisfies
    \begin{equation} \max_{a\leq x\leq b}|y(x_n)-w_n| \leq e^{(b-a)L}|y_0-w_0|+\left[\frac{e^{(b-a)L}-1}{L} \right]\tau(h)\end{equation}
    where
    \begin{equation}\tau(h) = \max_{a\leq x\leq b}|\tau_n(h)|,\end{equation}
    If the consistency condition 
    \begin{equation} \delta(h) \rightarrow 0 \mbox{ as  } h\rightarrow 0, \end{equation}
    where
    \begin{equation}\delta(h) = \max_{a \leq x \leq b}|f(x,y)-F(x,y;h;f)|. \end{equation}


## Question 6

6. Adapt the Python code for the Heun’s second order Runge-Kutta method provided to approximate solution of the integrate and fire differential equation:
    \begin{equation}   \tau_m\frac{dV}{dt} = -(V-E_L) + R_mI(t), \ \ -50\leq t \leq 400, \end{equation}

    where $E_L = -75$, $\tau_m = 10$,
    $R_m = 10$ and $I(t)=0.01t$
    and the initial condition
    $V(-50) = -75$ using a stepsize of $h=0.5$.