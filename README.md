# ThermoState

This package provides a wrapper around [CoolProp](https://github.com/CoolProp/CoolProp) that integrates [Pint](https://pint.readthedocs.io) for easy thermodynamic state management in any unit system.

## Installation

### Conda

The preferred installation method is to use [`conda`](https://anaconda.com/download). Using Conda, ThermoState can be installed for Python 3.7 or higher. If you have an existing Conda environment with one of those Python versions, installing ThermoState can be done by:

```bash
conda install -c conda-forge thermostate
```

This installs ThermoState and its dependencies from the `conda-forge` channel.

If you do not have an environment with Python 3.7 or higher, you can create a new environment with:

```bash
conda create -n thermostate -c conda-forge thermostate
```

### Pip

Alternatively, ThermoState can be installed with pip.

```bash
python -m pip install thermostate
```

Note that for versions of Python >= 3.9, CoolProp 6.4.1 will not work from PyPI. You'll
need to install CoolProp from their source repository until CoolProp >6.4.1 is
released. In this case, you can still install ThermoState from PyPI by specifying
not to install the dependencies automatically:

```bash
python -m pip install --no-deps thermostate matplotlib numpy pint
```

Then you'll need to install CoolProp into the same environment separately. Note that the conda package is available for all Python versions after 3.7.

### From Source

ThermoState is a pure-Python package that supports any Python version 3.7 and higher. To install from source, clone the source code repository and install using `pip`.

```bash
git clone https://github.com/bryanwweber/thermostate
cd thermostate
pip install .
```

## Documentation

Documentation can be found at <https://thermostate.readthedocs.io/>. The documentation contains a short [tutorial](https://thermostate.readthedocs.io/en/stable/Tutorial.html), [examples](https://thermostate.readthedocs.io/en/stable/examples.html), and [API documentation](https://thermostate.readthedocs.io/en/stable/thermostate.html) for the package.

[![Documentation Status](https://readthedocs.org/projects/thermostate/badge/?version=stable)](https://thermostate.readthedocs.io/en/stable/?badge=stable)

## Citation

If you have used ThermoState in your work, we would appreciate including a citation to the software! ThermoState has been published in [JOSE](https://jose.theoj.org/), available at the link below.

[![DOI](https://jose.theoj.org/papers/10.21105/jose.00033/status.svg)](https://doi.org/10.21105/jose.00033)

For those using Bib(La)TeX, you can use the following entry

```bibtex
@article{weber_thermostate_2018,
    title = {{ThermoState}: {A} state manager for thermodynamics courses},
    volume = {1},
    issn = {2577-3569},
    shorttitle = {{ThermoState}},
    url = {https://jose.theoj.org/papers/10.21105/jose.00033},
    doi = {10.21105/jose.00033},
    number = {8},
    urldate = {2018-10-24},
    journal = {Journal of Open Source Education},
    author = {Weber, Bryan},
    month = oct,
    year = {2018},
    pages = {33}
}
```

## Code of Conduct & Contributing

We welcome contributions from anyone in the community. Please look at the [Contributing instructions](https://github.com/bryanwweber/thermostate/blob/master/CONTRIBUTING.md) for more information. This project follows the [Contributor Covenant Code of Conduct](https://github.com/bryanwweber/thermostate/blob/master/CODE_OF_CONDUCT.md), version 1.4\. In short, be excellent to each other.

## Continuous Integration Status

[![codecov](https://codecov.io/gh/bryanwweber/thermostate/branch/master/graph/badge.svg)](https://codecov.io/gh/bryanwweber/thermostate)[![Python package](https://github.com/bryanwweber/thermostate/workflows/Python%20package/badge.svg)](https://github.com/bryanwweber/thermostate/actions?query=workflow%3A%22Python+package%22)

## Anaconda Package Version

[![Anaconda-Server Badge Version](https://anaconda.org/bryanwweber/thermostate/badges/version.svg)](https://anaconda.org/bryanwweber/thermostate) [![Anaconda-Server Badge Downloads](https://anaconda.org/bryanwweber/thermostate/badges/downloads.svg)](https://anaconda.org/bryanwweber/thermostate)
