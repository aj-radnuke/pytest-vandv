# pytest-vandv
A `pytest` plugin for importing (potentially large) datasets to validate
numerical computations.

**NOTE: The initial beta version of this plugin is currently in active**
**development; stay tuned for the first release!**

## Overview
This plugin intends to serve as a mechanism for verification and validation
(V&V) of programs that perform numerical computation.
Other `pytest` plugins for loading data and performing comparisons do exist
[^1].
`pytest-vandv`, however, is is designed specifically for loading tabular data,
which may contain an arbitrary number of fields for input parameters and the
corresponding expected output values.
Additionally, this plugin recognizes that scientific and engineering codes may
require a large number (thousands or more) of parameterized cases for V&V
testing.
Thus, there is a design priority of efficiently processing these tables;
currently, `pandas` DataFrames are used for this purpose, but other backend
options may be added in the future.
Finally, `pytest-vandv` recognizes that the results from software V&V are often
delivered to program managers or others who may not have direct experience with
the code, so this plugin provides the option of compiling test results into
clear and compact (and good looking!) test reports in a variety of formats.

## Installing
This plugin will be available on PyPI for installing via `pip`.

## Usage
*in progress*

## Documentation
Once the initial beta release of this plugin is available, documentation will be
hosted on [Read the Docs](https://readthedocs.org).

## Roadmap
*in progress*

## Contributing
Once the initial beta release of this plugin is available, more information will
be provided on contributing!

[^1]: See, *e.g.*,
[pytest-arraydiff](https://pypi.org/project/pytest-arraydiff/),
[pytest-datafixtures](https://pypi.org/project/pytest-datafixtures/),
[pytest-filedata](https://pypi.org/project/pytest-filedata/),
[pytest-regressions](https://pypi.org/project/pytest-regressions/) (and most
likely, several others).