# Poisson Distribution

This repository focuses on the Poisson Distribution, a probability distribution that expresses the probability of a given number of events occurring in a fixed interval of time or space, assuming these events occur with a known constant mean rate and independently of the time since the last event.

## Prerequisites

- Python 3.6 or higher
- Libraries: numpy, matplotlib

## Installation

To use the code examples in this repository, you will need to install the necessary Python libraries:

```bash
pip install numpy matplotlib
```

## Example - Poisson Distribution Calculation and Visualization

This example demonstrates how to compute and visualize Poisson probabilities using NumPy and Matplotlib.

### `poisson_example.py`

```python
import numpy as np
import matplotlib.pyplot as plt

# Probability of k events in a fixed interval
lambda_ = 4  # average number of events per interval
k_values = np.arange(0, 10)  # possible number of events
poisson_probabilities = np.exp(-lambda_) * np.power(lambda_, k_values) / np.factorial(k_values)

# Plotting the distribution
plt.bar(k_values, poisson_probabilities, color='blue', alpha=0.7)
plt.title('Poisson Distribution - $\lambda=4$')
plt.xlabel('Number of Events')
plt.ylabel('Probability')
plt.show()
```

## Contributing

Contributions that improve the clarity of explanations, extend the range of examples, or enhance the visualization of data are welcome. Please fork this repository, create a new branch for your changes, and submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
