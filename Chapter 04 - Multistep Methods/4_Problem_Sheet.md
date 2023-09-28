<!-- #region -->
# Problem Sheet 4 - Multistep Methods
## Question 1

1. 
    a. Apply the 3-step Adams-Bashforth to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution:
    \begin{equation} y'=t-y, \ \ (0\leq t \leq 4),\end{equation}
    with the initial condition $y(0)=1,$
    Let $N=4$,  with the exact solution
    \begin{equation}y(t)=2e^{-t}+t-1.\end{equation}


    b. Apply the 3-step Adams-Bashforth to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution:
    \begin{equation}y'=y-t, \ \ (0\leq t \leq 2),\end{equation}
    with the initial condition $y(0)=2,$
    Let $N=4$, with the exact solution
    \begin{equation}y(t)=e^{t}+t+1.\end{equation}

## Question 2


2. 
    a. Apply the 2-step Adams-Moulton Method to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution:
    \begin{equation} y'=t-y, \ \ (0\leq t \leq 4),\end{equation}
    with the initial condition $y(0)=1,$
    Let $N=4$,  with the exact solution
    \begin{equation}y(t)=2e^{-t}+t-1.\end{equation}

    b. Apply the 3-step Adams-Moulton Method to approximate the solution of the given initial value problems using the indicated number of time steps. Compare the approximate solution with the given exact solution:
    \begin{equation}y'=y-t, \ \ (0\leq t \leq 2),\end{equation}
    with the initial condition $y(0)=2,$
    Let $N=4$, with the exact solution
    \begin{equation}y(t)=e^{t}+t+1.\end{equation}


## Question 3


3. Derive the difference equation for the 1-step Adams-Bashforth method:
\begin{equation} w_{n+1}=w_n+hf(t_{n},w_{n}),\end{equation}
with the local truncation error
\begin{equation} \tau_{n+1}(h)=\frac{h}{2}y^{2}(\mu_n),\end{equation}
where $\mu_n \in (t_{n},t_{n+1})$.

## Question 4

4. Derive the difference equation for the 2-step Adams-Bashforth method:
\begin{equation} w_{n+1}=w_n+(\frac{3}{2}hf(t_{n},w_{n})-\frac{1}{2}hf(t_{n-1},w_{n-1})),\end{equation}
with the local truncation error
\begin{equation} \tau_{n+1}(h)=\frac{5h^2}{12}y^{3}(\mu_n),\end{equation}
where $\mu_n \in (t_{n-1},t_{n+1})$.


## Question 5

5. Derive the difference equation for the 2-step Adams-Moulton method:
\begin{equation} w_{n+1}=w_n+hf(t_{n+1},w_{n+1}),\end{equation}
with the local truncation error
\begin{equation}\tau_{n+1}(h)=-\frac{h}{2}y^{2}(\mu_n),\end{equation}
where $\mu_n \in (t_{n-2},t_{n+1})$.

## Question 6

6. Adapt the Python code for the 2-step Adams-Bashforth method provided to approximate solution of the integrate and fire differential equation:
   \begin{equation} \tau_m\frac{dV}{dt} = -(V-E_L) + R_mI(t),  \ \ -50\leq t \leq 400, \end{equation}
    where $E_L = -75$, $\tau_m = 10$,
    $R_m = 10$ and $I(t)=0.01t$
    and the initial condition
    $V(-50) = -75$ using a stepsize of $h=0.5$.
 

## Question 7


7. 

a. Define in your own words the terms strongly stable, weakly stable and unstable with respect to the characteristic equation.

b. Show that the two step Adams-Bashforth method is strongly stable.

## Question 8
Apply the Predictor-Corrector method to numerically approximate the solution at $x=1.0$ of the Initial Value Problem
\begin{equation}\frac{dy}{dx}=-y+x^2, \ \  0\leq x \leq 1,  \ \ \ y(0) = 1, \ \ \ y(0.25)=0.65, \end{equation}
using the two step Adams-Bashforth method and the one step Adams-Moulton method
\begin{equation} w_{i+1}=w_i + \frac{h}{2}[f(x_{i+1},w_{i+1})+f(x_{i},w_{i})], \end{equation}
with a step size of $h=0.25$.

## Question 9


9.  In your own words discuss the following concepts and their relevance for the
Adams-Bashforth and Adams-Moulton methods for approximating the solution
to initial value problems:

a. implicit and explicit numerical methods;

b. consistency of the numerical methods; 

c. convergence of the numerical methods; 

d. stability of the numerical methods. 

Illustrate your answers by stating conditions which are required.
