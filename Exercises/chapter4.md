# Conceptual

## 5.1
$$\\
\begin{aligned}\\
    1 - p(X) &= \frac{1}{1+e^{\beta_0 + \beta_1 X}} \\
    \frac{p(X)}{1-p(X)} &= 1+e^{\beta_0 + \beta_1 X}

\end{aligned}
$$

<!-- ## 5.2 
Since all the terms not relative to $k$ are constants including $x$,
$$\\
\begin{aligned}\\
    \argmax _k {logP_k(X)} &= \argmax _k [\log{\pi_k} - \frac{1}{2\sigma^2} (x - \mu_k)^2 ] \\
                           &= \argmax _k [\log{\pi_k} + \frac{\mu_k x}{\sigma^2} - \frac{\mu_k^2}{2\sigma^2} ]
\end{aligned}
$$ -->


## 5.2
Since all the terms not relative to $k$ are constants,
$$\\
\begin{aligned}\\
    \argmax _k {logP_k(X)} &= \argmax _k [\log{\pi_k} - \frac{1}{2\sigma^2} (x - \mu_k)^2 ] \\
                           &= \argmax _k [\log{\pi_k} + \frac{\mu_k x}{\sigma^2} - \frac{\mu_k^2}{2\sigma^2} ]
\end{aligned}
$$

## 5.3
Since all the terms not relative to $k$ are constants,
$$\\
\begin{aligned}\\
    \argmax _k {logP_k(X)} &= \argmax _k [\log{\pi_k} - \frac{1}{2\sigma_k^2} (x - \mu_k)^2 ] \\
                           &= \argmax _k [-\frac{x^2}{2\sigma_k^2} + \frac{\mu_k x}{\sigma_k^2} - \frac{\mu_k^2}{2\sigma^2} + \log{\pi_k}]
\end{aligned}
$$

which is a qudratic function of $x$


## 5.4