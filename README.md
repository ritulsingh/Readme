# Number System Converter
[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)]()
[![Python 3.8+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)


<span style="font-size:1.5em;">`number-system` is a Python 3.7+ package that simplifies the task of converts the decimal number in binary, octal, and hexadecimal or vice versa.
  
<span style="font-size:1.5em;">The number system or the numeral system is the system of naming or representing numbers. There are various types of number systems in maths like binary, decimal, etc.</span>


## Contents
- [Types](##-Types)
- [Installation](#-installation)
- [Quick Start](#-quick-start)
- [Contribute](#-contribute)
- [Conferences and Meet-ups](#-conferences-and-meet-ups)
- [Citation](#-citation)
- [Developers and Maintainers](#-developers-and-maintainers)
- [Acknowledgements](#-acknowledgements)
- [Copyright](#-copyright)


## Types
There are various types of the number system in mathematics. The four most common number system types are:
 1. Decimal number system (Base- 10)
 2. Binary number system (Base- 2)
 3. Octal number system (Base-8)
 4. Hexadecimal number system (Base- 16)

  #### Main Features
  * Interfaces with `scikit-learn` to provide a customer-centric and efficient way to perform imputation using machine learning algorithms.
  * Support for numerous imputation strategies and performance metrics, as specified below:


  #### Imputation Strategies

  | Univariate            | Generalised Linear Models   | Bagging and Boosted Trees    | Neural Nets
  | :---------------------| :-------------------------- | :----------------------------| :-----------------------
  | Mean                  | Linear Regressions          | Bagging Regressor            | Multi-layer Perceptron
  | Median                | Lasso                       | Extra Trees Regressor        |
  | Mode                  | Ridge                       | Extreme Gradient Boosting    |
  |                       |                             | Random Forest Regressor      |
  |                       |                             | XGBoost, LightGBM, CatBoost  |


  #### Performance Metrics
  |                       |
  | :---------------------|
  | Simple error           |
  | Percentage error      |
  | Naive forecasting          |
  | Relative Error      |
  | Bounded Relative Error         |
  | Geometric mean      |
  | Mean Squared Error          |
  | Normalized Root Mean Squared Error      |
  | Mean Error         |
  | Mean Absolute Error      |
  | Geometric Mean Absolute Error         |
  | Median Absolute Error      |
  | Mean Percentage Error |
  | Mean Absolute Percentage Error |
  | Median Absolute Percentage Error |
  | Symmetric Mean Absolute Percentage Error |
  | Symmetric Median Absolute Percentage Error |
  | Mean Arctangent Absolute Percentage Error |
  | Mean Absolute Scaled Error |
  | Normalized Absolute Error |
  | Normalized Absolute Percentage Error |
  | Root Mean Squared Percentage Error |
  | Root Median Squared Percentage Error |
  | Root Mean Squared Scaled Error |
  | Integral Normalized Root Squared Error |
  | Root Relative Squared Error |
  | Mean Relative Error |
  | Median Relative Absolute Error |
  | Geometric Mean Relative Absolute Error |
  | Mean Bounded Relative Absolute Error |
  | Unscaled Mean Bounded Relative Absolute Error |
  | Mean Directional Accuracy  |


  #### Versions and Dependencies
  * Python 3.7+
  * Dependencies:
      - `missingno` >= 0.4.1
      - `numpy` >= 1.15.4
      - `pandas` >= 0.20.3
      - `scikit-learn` >= 0.20.2
      - `xgboost` >= 0.83


## Installation
There are two ways to install the `PyImpuyte` package:

- Install `PyImpuyte` from PyPI (recommended):
```
pip install PyImpuyte==1.3.5
```
- Install `PyImpuyte` from the Bitbucket source:
```
git clone https://bitbucket.csiro.au/scm/dde/pyimpuyte.git
cd pyimpuyte
python setup.py install
```


## Quick Start
To start imputing missing values with `PyImpuyte`, a `config.json` file must be passed. The following workflow can be used:

```config.json
{
    "pyimpuyte": {
        "input": [
            "data/synth_data_test.csv"
        ],
        "feature_list": ["TURNOVER", "WAGES", "SALES"],
        "target": "FTE",
        "skip_columns": null,
        "nrows": 1000,
        "drop_duplicates": true,
        "output": "out/synth_data_test.csv",
        "evaluation": "out/evaluation.csv"
    }
}
```
## Run PyImpuyte
To run `PyImpuyte`, excute the following command from the terminal"
```
pyimpuyte\imputer.py config.json
```

For more information about how to configure `PyImpuyte`, see our suggested **[template](https://bitbucket.csiro.au/projects/DDE/repos/pyimpuyte/browse/config.md)**.


## Contribute
We welcome all kinds of contributions that improve the performance of the currently published pacakge. See the [Contribution Guide](https://bitbucket.csiro.au/projects/DDE/repos/pyimpuyte/browse/CONTRIBUTING.md) for more details.


## Conferences and Meet-ups
* We presented our research at the **[2019 Australasian Joint Conference on Artificial Intelligence](http://nugget.unisa.edu.au/AI2019/index.php)** which lead to the development of `PyImpuyte`.

* We will be presenting at the next Canberra Data Scientists Meet-up on 28 July 2020.


## Citation
Please cite our work in your publications if it helps your research.

* Conference Paper - Chapter 18 of **[AI2019: Advances in Artificial Intelligence](https://link.springer.com/chapter/10.1007/978-3-030-35288-2_18)**.

```BibTeX
@inbook{inbook,
  author = {Suresh, Marcus and Taib, Ronnie and Zhao, Yanchang and Jin, Warren},
  year = {2019},
  month = {11},
  pages = {215-227},
  title = {Sharpening the BLADE: Missing Data Imputation Using Supervised Machine Learning},
  isbn = {978-3-030-35287-5},
  doi = {10.1007/978-3-030-35288-2_18}
}
```

* Python Package - **[PyImpuyte](https://bitbucket.csiro.au/projects/DDE/repos/pyimpuyte)**.

```BibTeX
@misc{Suresh2020_PyImpuyte,
  title={PyImpuyte},
  author={Suresh, Marcus et al.},
  year={2020},
  howpublished={\url{https://bitbucket.csiro.au/projects/DDE/repos/pyimpuyte}},
}
```


## Developers and Maintainers
* The developers began work to bring `PyImpuyte` into production in October 2019. `PyImpuyte` is actively maintained and there will be incremental improvements scheduled on a regular basis. The lead developers and maintainers are:

  * <b>Marcus Suresh</b>, Bitbucket: [sur033](https://bitbucket.csiro.au/users/sur033) and GitHub: [marcus-suresh](https://github.com/marcus-suresh)

  * <b>Ronnie Taib</b>, GitHub: [rtaib](https://github.com/rtaib)

* See the [Developers](https://bitbucket.csiro.au/projects/DDE/repos/pyimpuyte/browse/DEVELOPERS.rst) page to get in touch with the `PyImpuyte` team.


## Acknowledgements
* This research was funded by the Australian Government through the [Department of Industry, Science, Energy and Resources (DISER)](https://www.industry.gov.au/) and the [Data Integration Partnership for Australia (DIPA)](https://www.pmc.gov.au/public-data/data-integration-partnership-australia).

* The developers would like to extend their gratitude to Dr. Abrie Swanepoel (Branch Manager) and Dr. Tala Talgasawatta (Director) from DISER for their ongoing support in `PyImpuyte`.


## Copyright
`PyImpuyte` is distributed under the MIT license. See [LICENSE](https://bitbucket.csiro.au/projects/DDE/repos/pyimpuyte/browse/LICENSE) for details.
