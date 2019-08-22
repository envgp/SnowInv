# SnowInv

## Disk Load

For a disk load of unit weight (force), the solution from Farrell 72 is:
    
\begin{equation}
u(0,r) =
    \begin{cases}
    -\frac{\sigma}{\pi^2\mu\eta \alpha} E\big(\frac{r}{
    \alpha} \big) & r < \alpha \\
    -\frac{\sigma r}{\pi^2\mu\eta \alpha^2} \Big\lbrack E\big(\frac{\alpha}{
    r}\big) - \big( 1 - \frac{\alpha^2}{r^2} K\big(\frac{\alpha}{r}\big) \Big\rbrack & r > \alpha
    \end{cases}
\end{equation}

where $E(x)$ and $K(x)$ are the complete elliptic integrals, which are a special function commonly tabulated (and included in scipy). As for constants, $\mu$ is the shear modulus, $\lambda$ is Lame's first parameter, $\eta = \mu + \lambda$ and $\alpha$ is the disk radius.

This scenario is also derived in Contact Mechanics, in terms of Young's Modulus and Poisson's Ratio, but I haven't gone through it in detail. The relationship between YM, Poisson's Ratio and Lame Parameters amongst more is here:

