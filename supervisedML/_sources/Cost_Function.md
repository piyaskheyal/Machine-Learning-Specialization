# Cost Function: Squared Error Cost Function

In linear regression, the **cost function** quantifies how well the model's predictions align with the actual data. The squared error cost function is commonly used and defined as follows:

## Definition
The cost function \( J(w, b) \) is given by:

$$
J(w, b) = \frac{1}{2m} \sum_{i=1}^{m} \left( f_{w, b}(x^{(i)}) - y^{(i)} \right)^2
$$

Where:
- $m$ is the number of training examples.
- $f_{w, b}(x^{(i)})$ is the predicted value for the $i$-th training example.
- $y^{(i)}$ is the actual value for the $i$-th training example.
- $w$ and $b$ are the model parameters (weights and bias).

## Intuition
- The term $f_{w, b}(x^{(i)}) - y^{(i)}$ is the error (difference between prediction and actual value) for the $i$-th training example.
- Squaring this error ensures all differences are positive and emphasizes larger errors.
- Dividing by $2m$ simplifies the gradient calculations in the optimization process.

Minimizing this cost function using methods like **gradient descent** helps the model achieve better performance by adjusting $w$ and $b$ appropriately.