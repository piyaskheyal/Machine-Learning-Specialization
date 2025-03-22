### Standard Deviation

The **standard deviation** is a measure of the spread or dispersion of a set of values in a dataset. It indicates how much individual data points deviate from the mean. A low standard deviation means the data points are close to the mean, while a high standard deviation means the data points are spread out over a wider range of values.

#### Formula:
$$ 
\sigma = \sqrt{\frac{1}{N} \sum_{i=1}^{N} (X_i - \mu)^2} 
$$

Where:
- $ \sigma $ is the standard deviation.
- $ N $ is the number of data points.
- $ X_i $ is each data point.
- $ \mu $ is the mean of the data.

#### What it does:
- **Squaring the deviations**: It measures the deviation of each data point from the mean, ensuring all deviations are positive.
- **Taking the square root**: This step brings the units of the result back to the original units of the data, ensuring the standard deviation is interpretable in the same scale as the dataset.

The standard deviation is useful in various contexts, including statistical analysis, probability theory, and machine learning, as it helps assess the variability or risk in the data.