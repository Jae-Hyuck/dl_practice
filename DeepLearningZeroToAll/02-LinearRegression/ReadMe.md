# Linear Regression

## (Linear) Hypothesis

$$
H(x) = Wx + b
$$

어떤 $W$와 $b$를 가지는 Hypothesis가 가장 데이터에 잘 맞는지 찾아야 한다.

## Cost (Loss) Function

우리가 세운 가설과 실제 데이터가 얼마나 다른가?

예를 들어,

$$
cost(W, b) = \frac{1}{m} \sum_{i=1}^{m} (H(x^{(i)})-y^{(i)})^2
$$

## Goal

cost를 최소화하는 $W$, $b$를 찾는다. (Gradient descent algorithm으로 가능)

## Multi Variable Linear Regression

#### 2변수

$$
H(x_1,x_2) = w_1 x_1 + w_2 x_2 + b
$$

$$
cost(W,b) = \frac{1}{m} \sum_{i=1}^m (H(x_1^{(i)}, x_2^{(i)}) - y^{(i)})^2
$$

#### 다변수 (as matrix form)

$$
H(x_1, x_2, x_3) =
\begin{bmatrix}
b & w_1 & w_2 & w_3 \\
\end{bmatrix}
\times
\begin{bmatrix}
1 \\ x_1 \\ x_2 \\ x_3 \\
\end{bmatrix}
$$

$$
H(X) = W^T X
$$

$W$에 bias term이 포함 되었음을 유의

## 이 때의 Gradient Descent의 Update Rule

$$
W := W - \alpha \frac{\partial}{\partial W} cost(W)
$$



