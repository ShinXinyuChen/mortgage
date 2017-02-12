Mortgage
====================

[![Travis](https://img.shields.io/travis/austinmcconnell/mortgage.svg)](https://travis-ci.org/austinmcconnell/mortgage)

[![Codecov](https://img.shields.io/codecov/c/github/austinmcconnell/mortgage.svg)](https://codecov.io/gh/austinmcconnell/mortgage)

[![Pyup](https://pyup.io/repos/github/austinmcconnell/mortgage/shield.svg)](https://pyup.io/repos/github/austinmcconnell/mortgage/)

Simple mortgage calculator tool


Installation
--------------------

How To Use
--------------------

This package is intended to help understand the true cost of a mortgage. It also can help you easily compare between different mortgages.
 
Begin by importing the loan class

```python
from mortgage import Loan

``` 

Create a simple mortgage

```python
loan = Loan(principal=200000, interest=.06, term=30, start_date=(2017,3,1))
```

View a summary of pertinent mortgage information by calling the summarize property.

```python
loan.summarize

>>> Original Balance:         $    200,000
>>> Interest Rate:                    0.06 %
>>> APY:                              6.17 %
>>> APR:                              6.00 %
>>> Term:                               30 years
>>> Monthly Payment:          $    1199.10

>>> Total principal payments: $ 200,000.00
>>> Total interest payments:  $ 231,676.38
>>> Total payments:           $ 431,676.38
>>> Interest to principal:           115.8 %
>>> Years to pay:                     30.0
```


Run The Test Cases
--------------------
From the top level directory, run the following command:

```
pytest
```
