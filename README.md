# JGB_distributions


## Description

JGB_distributions is a Python library for dealing with Gaussian (normal) and Binomial Probability distributions.

## Files

Generaldistribution.py: generic distribution class 

Binomialdistribution.py: Binomial distribution class for calculating and 
    visualizing a Binomial distribution.

Gaussiandistribution.py: Gaussian distribution class for calculating and 
    visualizing a Gaussian distribution.


## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install JGB_distributions.

```bash
pip install JGB_distributions
```

## Usage

```python
import JGB_distributions

# returns 'mean, standard deviation of a Gaussian distributions'
G = JGB_distributions.Gaussian(mean, stdev)

# returns 'mean, standard deviation, probability and size of a Binomial distributions'
B = JGB_distributions.Binomial(prop, n)

# returns 'mean, standard deviation of a Gaussian distributed data'
G.read_data_file(file_name)

# returns 'mean, standard deviation, probability and size of a Binomial distributed data'
B = JGB_distributions.Binomial()
B.read_data_file(file_name)
B.replace_stats_with_data()

# to calculate the mean for a dataset
G.calculate_mean()
B.calculate_mean()

# to calculate the standard deviation for the two distributions
G.calculate_stdev()
B.calculate_stdev()

# to plot the distributions
G.plot_histogram()
B.plot_bar()

# to calculate Probability density function  for the two distributions
G.pdf(point)
B.pdf(point)

# to plot Probability density function  for the two distributions
G.plot_histogram_pdf(number of data points)
B.plot_bar_pdf()

# to add two distributions of the same type
G_1 + G_2
B_1 + B_2
```

## License
This project is licensed under the [MIT](https://choosealicense.com/licenses/mit/) - see the License.txt file for details

