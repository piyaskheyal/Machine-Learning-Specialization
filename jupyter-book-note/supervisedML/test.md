# Gradient Descent for Multivariable Cost Functions

## **Cost Function**  
For a model with multiple weights (**vectorW**) and a bias term $b$, the cost function $J(\mathbf{w}, b)$ quantifies the error between predictions $h_{\mathbf{w},b}(\mathbf{x})$ and true labels $y$. For linear regression:  
$$
J(\mathbf{w}, b) = \frac{1}{2m} \sum_{i=1}^m \left( h_{\mathbf{w},b}(\mathbf{x}^{(i)}) - y^{(i)} \right)^2
$$  
where $h_{\mathbf{w},b}(\mathbf{x}) = \mathbf{w} \cdot \mathbf{x} + b$.

---

## **Gradient Descent Steps**  
To minimize $J(\mathbf{w}, b)$:  
1. **Initialize** weights $\mathbf{w}$ and bias $b$.  
2. **Compute partial derivatives** of $J$ with respect to each parameter:  
   - For each weight $w_j$:  
   $$
   \frac{\partial J}{\partial w_j} = \frac{1}{m} \sum_{i=1}^m \left( h_{\mathbf{w},b}(\mathbf{x}^{(i)}) - y^{(i)} \right) x_j^{(i)}
   $$  
   - For bias $b$:  
   $$
   \frac{\partial J}{\partial b} = \frac{1}{m} \sum_{i=1}^m \left( h_{\mathbf{w},b}(\mathbf{x}^{(i)}) - y^{(i)} \right)
   $$  
3. **Update parameters simultaneously**:  
   $$
   w_j := w_j - \alpha \frac{\partial J}{\partial w_j} \quad \text{(for all $j$)}
   $$  
   $$
   b := b - \alpha \frac{\partial J}{\partial b}
   $$  
4. **Repeat** until convergence (small changes in $J$).  

---

## **Key Notes**  
- **Learning Rate ($\alpha$)**: Controls step size. Too small → slow convergence; too large → overshooting.  
- **Feature Scaling**: Normalize features to ensure gradients update weights uniformly.  
- **Convergence**: Track $J(\mathbf{w}, b)$ or parameter changes (e.g., $\Delta \mathbf{w} < \epsilon$).  
- **Vectorization**: Use matrix operations (e.g., NumPy) for efficient computation.  