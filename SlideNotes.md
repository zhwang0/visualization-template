
# Logistic Regression as a Neural Network

## Binary Classification

**Notations:**

- Dataset:  $(x,y), x\in \mathbb{R}^{n_{x}}, y \in \{0, 1\}$, where $n_{x}$ is the number of pixels in all bands

- Training and Testing data: $ m_{train/test} = \{(x^{1}, y^{1}), ..., (x^{m}, y^{m}) \} $

- Input data for neural network: 
    - $$X = [x^{1}, x^{2}, ..., x^{m}] $$
    where $X \in \mathbb{R}^{n_{x} \times m}$
    
    - $$Y = [y^{1}, y^{2}, ..., y^{m}] $$
    where $X \in \mathbb{R}^{1 \times m}$

## Logistic Regression

**Basic Concept:**


- Given $X$ wants $\hat{y} = P(y=1 | x)$

    where $X \in \mathbb{R}^{n_{x}}$, $0 \leq \hat{y} \leq 1$
- Parameters: $\underline{\omega} \in \mathbb{R}^{n_{x}}$, $b \in \mathbb{R}$


- Outputs: 

    $ \hat{y} = \sigma \: ( \omega ^{T}x + b) $

    where $ \sigma(z) = \frac{1}{1 + e^{-z}} $
    
    <img src = 'imgs\sigmoid.png'>
    

## Logistic Regression Cost Function

**Loss (Error) Function:**

$$\mathcal{L} (\hat{y}, y) = -( y \;\log \hat{y} + ( 1 - y) \; log( 1 - \hat{y}) ) $$


**Cost Function:**

$$J(w,b) = \frac{1}{m} \; \sum _{i=1}^{m} \mathcal{L} (\hat{y} \; ^{(i)}, y^{(i)}) = - \frac{1}{m} \; \sum _{i=1}^{m}[ y^{(i)} \log \hat{y} \; ^{(i)} + ( 1 - y^{(i)} )  log( 1 - \hat{y} \; ^{(i)})) ]  $$

**Difference between Loss & Cost Function:**
- The loss function computes the error for a single training example
- The cost function is the average of the loss functions of the entire training set


## Gradient Descent

**Learn\Train the Parameters**

- Goal: want to find $w,b$ that minimize $J(w,b)$, which is defined as a convex function for simplfying the optimization

<img src = 'imgs\gd-ill.jpg'>

- Algorithm:

    Repeat:
$$w \: := \: w - \alpha \; \frac{\partial J(w,b)}{\partial w} $$
$$b \: := \: b - \alpha \; \frac{\partial J(w,b)}{\partial b} $$
    
    where $\alpha$ is the learning rate controlling how big a step we take on each iteration, $\frac{\partial J(w)}{\partial w}$, $dw$ used in the following section, is the partial derivative on $w$ representing the basic update or the change we want to make to the parameter $w$.


## Derivatives

## More Derivatives Examples

## Computation Graph

## Derivatives with a Computation Graph

## Logistic Regression Gradient Descent

## Gradient Descent on m Examples

-------

# Python and Vectorization



-----

# Quiz


