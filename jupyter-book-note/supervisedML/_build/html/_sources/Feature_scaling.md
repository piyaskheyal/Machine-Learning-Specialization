### Feature Scaling Techniques

#### 1. **Feature Scaling**
   - This technique scales the feature values by dividing them by the maximum value in the dataset. 
   - It results in a range from 0 to 1. This is useful when you need all features to be in the same range, especially for algorithms that are sensitive to the magnitude of values (e.g., KNN, gradient descent).
   - Formula:  
   
$$ 
\text{Scaled Feature} = \frac{X}{\max(X)} 
$$

#### 2. **Mean Normalization**
   - In this method, each feature value is adjusted by subtracting the mean and then dividing by the range (max - min) of the data.
   - Formula:  

$$ 
\text{Normalized Feature} = \frac{X - \text{mean}(X)}{\text{max}(X) - \text{min}(X)} 
$$
   - The result is a feature distribution between -0.5 and 0.5. This scaling is helpful when you want to center the data around zero.

#### 3. **Z-score Normalization (Standardization)**
   - This technique transforms the data by subtracting the mean and dividing by the standard deviation.
   - Formula:  

$$ 
Z = \frac{X - \mu}{\sigma} 
$$
   - It centers the data around zero and scales it based on its spread (standard deviation). This is useful for algorithms that assume normally distributed data or require data with zero mean and unit variance (e.g., linear regression, SVM).

To know more about **Standard Deviation**, [click here](Standard_deviation.md).