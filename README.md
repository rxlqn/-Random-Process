# Random Process learning notes

#### 2020\4\16

## Chapter 1

- **Characteristic function: $g(X) = e^{jtX}$**
  $$
  \Phi(t) = E\{e^{jtX}\}=\int_{-\infty}^{+\infty}e^{jtx}p(x)dx
  $$

  - 类比连续时间傅里叶变换$f(w)=\int_{-\infty}^{+\infty}e^{-jex}p(x)dx$

  - 随机变量$Z = X+Y$ :
    
    
    $$
    \begin{align}
    \Phi_{Z}(t) &= E\{{e^{jt(X+Y)}}\} \\
    &= E\{{e^{jtX}}\}*E\{e^{jtY}\}\\
    &= \Phi_X(t)*\Phi_Y(t)
    \end{align}
    $$
    

- For a nonnegative integer-valued random variable X it is often more convenient to work with the *z transform* of the pmf.

  **Moment-generating function:$g(x)=e^{sX}$**
  $$
  \Phi(s)=E\{{e^{sX}}\}=\int_{-\infty}^{+\infty}e^{sx}pxdx
  $$

  $$
  \begin{align}
  \Phi(s)&=E\{e^{sX}\}\\
  &=E\{1+sX+\frac{s^2}{2!}X^2+...\}\\
  &=1+sE\{X\}+\frac{s^2}{2!}E\{X^2\}+...
  \end{align}
  $$

  - so there is $E\{X^n\}=\frac{d^n}{ds^n}\Phi(s)|_{s=0}$

## Chapter 2

#### Frequently used distributions:

- **Bernoulli:**
  - pmf(probability mass function)