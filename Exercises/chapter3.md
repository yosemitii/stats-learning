# Conceptual

## 1. p-value
- Null hypothesis: There is no relationship between X and Y
- beta of  `TV` is significant non-zero
- beta of `radio` is significant non-zero
- bet of  `newspaper` is not significant


## 2.
- KNN regression: It uses the mean of k neareast neighbor as the the value of f(x)
  - It first identifies the K training observations that are closest to x0, represented by N0. 
  - It then estimates f(x0) using the average of all the training responses in N0. 
- KNN classifier: It uses the dominant members of the k nearest neighbors as its category.

## 3. 
(a) c. If GPA > 3.5, high - college = -35 + GPA * 10.
(b) 137.1
(c) No. It depends on the t-stats or p-value.

## 4. 
(a) Cubic regression can have lower RSS since the quadratic and cubic term allow it to fit more to the trainning set event it is overfitting.
(b) Linear regression has lower RSS. Overfit can reduce the trainning RSS but not testing RSS.
(c) not enough information to tell
(d) not enough information to tell


## 5. 
$a_i = \frac{x_i * \sum{(x_i')}}{\sum{(x_i'^2)}}$


## 6.
$\hat{y} = \hat{\beta_0} + \hat{\beta_1} * x$
plug in $\bar{x}$ and ${\beta_0}$, we obtain $\hat{y} = \bar{y} - \hat{\beta_1}\bar{x} + \hat{\beta_1}\bar{x} = \bar{y}$

## 7.
Given that, $\hat{\beta_1} = \frac{\sum(X_i-\bar{X})(Y_i-\bar{Y})}{(Y_i-\bar{Y})^2}$, $\hat{\beta_0} = \bar{y} - \hat{\beta_1}\bar{x}$

We obtain 
$$\\
\begin{aligned}\\
   RSS &= \sum_{i=1}^{n}(Y_i-\beta_0-\beta_1 X_i)^2\\
       &= \sum_{i=1}^{n}(Y_i-\bar{Y}+\hat{\beta_1}\bar{X}-\beta_1 X_i)^2 \\
       &= \sum_{i=1}^{n} \{(Y_i-\bar{Y})^2 + 2\hat{\beta_1}(Y_i-\bar{Y})(\bar{X}-X_i) + \hat{\beta_1}^2(X_i-\bar{X})^2 \} \\
\end{aligned}\\
$$

Since $TSS = \sum_{i=1}^{n} (Y_i-\bar{Y})^2 \\$
$$\\
\begin{aligned}\\
  TSS-RSS &= \sum_{i=1}^{n} \{2\hat{\beta_1}(Y_i-\bar{Y})(X_i-\bar{X}) - \hat{\beta_1}^2(X_i-\bar{X})^2 \} \\
          &= 2\frac{\sum_{i=1}^{n}(X_i-\bar{X})(Y_i-\bar{Y})}{\sum_{i=1}^{n}(X_i-\bar{X})^2}\cdot\sum_{i=1}^{n}(Y_i-\bar{Y})(X_i-\bar{X}) -\frac{\sum_{i=1}^{n}((X_i-\bar{X})(Y_i-\bar{Y}))^2}{\sum_{i=1}^{n}(X_i-\bar{X})^2}\\
          &=\frac{\sum_{i=1}^{n}((X_i-\bar{X})(Y_i-\bar{Y}))^2}{\sum_{i=1}^{n}(X_i-\bar{X})^2} \\
  \frac{TSS-RSS}{TSS} &= \frac{\sum_{i=1}^{n}((X_i-\bar{X})(Y_i-\bar{Y}))^2}{\sum_{i=1}^{n}(X_i-\bar{X})^2\cdot\sum_{i=1}^{n}(Y_i-\bar{Y})^2}\\
  % RSS = \sum_{i=1}^{n}(Y_i-\bar{Y}+\hat{\beta_1}\bar{X}-\beta_1 X_i)^2 \\  
  R^2 &= Corr(X,Y)^2\\
\end{aligned}\\
$$
