# CrossPy
The `CrossPy` package (short for _Cross_-validation in *Py*thon) is a package for performing cross-validation in Python.

### Contributors

* Nazli Ozum Kafaee / @nazliozum
* Daniel Raff / @raffrica
* Shun Chi / @ShunChi100

### Summary

Cross-validation is an important technique used in model selection and hyper-parameter optimization. Scores from cross-validation are a good estimation of test score of a predictive model in test data or new data as long as the IID assumption approximately holds in data. This package aims to provide a standardized pipeline for performing cross-validation for different modeling functions in Python. In addition, summary statistics of the cross-validation results are provided for users.  

### Functions

Three main functions in `CrossPy`:

- `train_test_split()`: This function split data according to input train/all ratio returns the split data. A random shuffling option is provided. (`stratification` option for imbalanced representations will also be included if time allows.)

- `cross_validation()`: This function performs `k`-fold cross validation using the partitioned data and a selected model. It returns the scores of each validation. Additional methods for cross validation will be implemented (such as "Leave-One-Out" if time allows).  

- `summary_cv()`: This function outputs summary statistics(mean, standard deviation, mode, median) of cross-validation scores.

### Similar packages

The [`scikit-learn`](http://scikit-learn.org/stable/) library in Python implements the first two functions we propose in [`sklearn.model_selection.train_test_split`](http://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) and [`sklearn.cross_validation`](http://scikit-learn.org/stable/modules/cross_validation.html). 


### License
[MIT License](https://github.com/UBC-MDS/CrossPy/blob/master/LICENSE)

### Contributing
This is an open source project. So feedback, suggestions and contributions are very welcome. For feedback and suggestions, please open an issue in this repo. If you are willing to contribute this package, please refer [Contributing](https://github.com/UBC-MDS/CrossPy/blob/master/CONTRIBUTING.md) guidelines for details.
