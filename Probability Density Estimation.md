# Probability Desnity Estimation

1. Assume the formula and parameter, try to fit the model. 
  * Cons: Not all data sets follow standard models.
2. 

# Kernel Estimation(Parzen-Rosenblatt Density Estimiation)
A non-parametric way to estimate the PDF of a randon variable. It is also called Parzen-Rosenblatt window method. 

## Assumptions
1. Given set of observations: $x_1, ...x_n$ iid random variables. 
2. They have same probability density function $f$, which is unknown. 

## Method 
Let h > 0,  
$$
 g_x(y) = \begin{cases}
            \frac{1}{2h},& y\in(x-h, x+h)\\ 
            0,& otherwise
            \end{cases}
$$

Define estimate of function f. 
$$
 \head{f}_n(y) = \frac{1}{n} \sum_{i=1}^n g_{X(i)}(y)
$$
