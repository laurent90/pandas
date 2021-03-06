<div align="center">
  <img src="https://github.com/pandas-dev/pandas/blob/master/doc/logo/pandas_logo.png"><br>
</div>

-----------------

# pandas: powerful Python data analysis toolkit

<table>
<tr>
  <td>Latest Release</td>
  <td><img src="https://img.shields.io/pypi/v/pandas.svg" alt="latest release" /></td>
</tr>
  <td></td>
  <td><img src="https://anaconda.org/conda-forge/pandas/badges/version.svg" alt="latest release" /></td>
</tr>
<tr>
  <td>Package Status</td>
  <td><img src="https://img.shields.io/pypi/status/pandas.svg" alt="status" /></td>
</tr>
<tr>
  <td>License</td>
  <td><img src="https://img.shields.io/pypi/l/pandas.svg" alt="license" /></td>
</tr>
<tr>
  <td>Build Status</td>
  <td>
    <a href="https://travis-ci.org/pandas-dev/pandas">
    <img src="https://travis-ci.org/pandas-dev/pandas.svg?branch=master" alt="travis build status" />
    </a>
  </td>
</tr>
<tr>
  <td></td>
  <td>
    <a href="https://circleci.com/gh/pandas-dev/pandas">
    <img src="https://circleci.com/gh/circleci/mongofinil/tree/master.svg?style=shield&circle-token=223d8cafa7b02902c3e150242520af8944e34671" alt="circleci build status" />
    </a>
  </td>
</tr>
<tr>
  <td></td>
  <td>
    <a href="https://ci.appveyor.com/project/pandas-dev/pandas">
    <img src="https://ci.appveyor.com/api/projects/status/86vn83mxgnl4xf1s/branch/master?svg=true" alt="appveyor build status" />
    </a>
  </td>
</tr>
<tr>
  <td>Coverage</td>
  <td><img src="https://codecov.io/github/pandas-dev/pandas/coverage.svg?branch=master" alt="coverage" /></td>
</tr>
<tr>
  <td>Conda</td>
  <td>
    <a href="http://pandas.pydata.org">
    <img src="http://pubbadges.s3-website-us-east-1.amazonaws.com/pkgs-downloads-pandas.png" alt="conda default downloads" />
    </a>
  </td>
</tr>
<tr>
  <td>Conda-forge</td>
  <td>
    <a href="http://pandas.pydata.org">
    <img src="https://anaconda.org/conda-forge/pandas/badges/downloads.svg" alt="conda-forge downloads" />
    </a>
  </td>
</tr>
<tr>
  <td>PyPI</td>
  <td>
    <a href="https://pypi.python.org/pypi/pandas/">
    <img src="https://img.shields.io/pypi/dm/pandas.svg" alt="pypi downloads" />
    </a>
  </td>
</tr>
</table>

[![https://gitter.im/pydata/pandas](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/pydata/pandas?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## What is it

**pandas** is a Python package providing fast, flexible, and expressive data
structures designed to make working with "relational" or "labeled" data both
easy and intuitive. It aims to be the fundamental high-level building block for
doing practical, **real world** data analysis in Python. Additionally, it has
the broader goal of becoming **the most powerful and flexible open source data
analysis / manipulation tool available in any language**. It is already well on
its way toward this goal.

## Main Features
Here are just a few of the things that pandas does well:

  - Easy handling of [**missing data**][missing-data] (represented as
    `NaN`) in floating point as well as non-floating point data
  - Size mutability: columns can be [**inserted and
    deleted**][insertion-deletion] from DataFrame and higher dimensional
    objects
  - Automatic and explicit [**data alignment**][alignment]: objects can
    be explicitly aligned to a set of labels, or the user can simply
    ignore the labels and let `Series`, `DataFrame`, etc. automatically
    align the data for you in computations
  - Powerful, flexible [**group by**][groupby] functionality to perform
    split-apply-combine operations on data sets, for both aggregating
    and transforming data
  - Make it [**easy to convert**][conversion] ragged,
    differently-indexed data in other Python and NumPy data structures
    into DataFrame objects
  - Intelligent label-based [**slicing**][slicing], [**fancy
    indexing**][fancy-indexing], and [**subsetting**][subsetting] of
    large data sets
  - Intuitive [**merging**][merging] and [**joining**][joining] data
    sets
  - Flexible [**reshaping**][reshape] and [**pivoting**][pivot-table] of
    data sets
  - [**Hierarchical**][mi] labeling of axes (possible to have multiple
    labels per tick)
  - Robust IO tools for loading data from [**flat files**][flat-files]
    (CSV and delimited), [**Excel files**][excel], [**databases**][db],
    and saving/loading data from the ultrafast [**HDF5 format**][hdfstore]
  - [**Time series**][timeseries]-specific functionality: date range
    generation and frequency conversion, moving window statistics,
    moving window linear regressions, date shifting and lagging, etc.


   [missing-data]: http://pandas.pydata.org/pandas-docs/stable/missing_data.html#working-with-missing-data
   [insertion-deletion]: http://pandas.pydata.org/pandas-docs/stable/dsintro.html#column-selection-addition-deletion
   [alignment]: http://pandas.pydata.org/pandas-docs/stable/dsintro.html?highlight=alignment#intro-to-data-structures
   [groupby]: http://pandas.pydata.org/pandas-docs/stable/groupby.html#group-by-split-apply-combine
   [conversion]: http://pandas.pydata.org/pandas-docs/stable/dsintro.html#dataframe
   [slicing]: http://pandas.pydata.org/pandas-docs/stable/indexing.html#slicing-ranges
   [fancy-indexing]: http://pandas.pydata.org/pandas-docs/stable/indexing.html#advanced-indexing-with-ix
   [subsetting]: http://pandas.pydata.org/pandas-docs/stable/indexing.html#boolean-indexing
   [merging]: http://pandas.pydata.org/pandas-docs/stable/merging.html#database-style-dataframe-joining-merging
   [joining]: http://pandas.pydata.org/pandas-docs/stable/merging.html#joining-on-index
   [reshape]: http://pandas.pydata.org/pandas-docs/stable/reshaping.html#reshaping-and-pivot-tables
   [pivot-table]: http://pandas.pydata.org/pandas-docs/stable/reshaping.html#pivot-tables-and-cross-tabulations
   [mi]: http://pandas.pydata.org/pandas-docs/stable/indexing.html#hierarchical-indexing-multiindex
   [flat-files]: http://pandas.pydata.org/pandas-docs/stable/io.html#csv-text-files
   [excel]: http://pandas.pydata.org/pandas-docs/stable/io.html#excel-files
   [db]: http://pandas.pydata.org/pandas-docs/stable/io.html#sql-queries
   [hdfstore]: http://pandas.pydata.org/pandas-docs/stable/io.html#hdf5-pytables
   [timeseries]: http://pandas.pydata.org/pandas-docs/stable/timeseries.html#time-series-date-functionality

## Where to get it
The source code is currently hosted on GitHub at:
http://github.com/pandas-dev/pandas

Binary installers for the latest released version are available at the [Python
package index](http://pypi.python.org/pypi/pandas/) and on conda.

```sh
# conda
conda install pandas
```

```sh
# or PyPI
pip install pandas
```

## Dependencies
- [NumPy](http://www.numpy.org): 1.7.0 or higher
- [python-dateutil](http://labix.org/python-dateutil): 1.5 or higher
- [pytz](http://pytz.sourceforge.net)
    - Needed for time zone support with ``pandas.date_range``

See the [full installation instructions](http://pandas.pydata.org/pandas-docs/stable/install.html#dependencies)
for recommended and optional dependencies.

## Installation from sources
To install pandas from source you need Cython in addition to the normal
dependencies above. Cython can be installed from pypi:

```sh
pip install cython
```

In the `pandas` directory (same one where you found this file after
cloning the git repo), execute:

```sh
python setup.py install
```

or for installing in [development mode](https://pip.pypa.io/en/latest/reference/pip_install.html#editable-installs):

```sh
python setup.py develop
```

Alternatively, you can use `pip` if you want all the dependencies pulled
in automatically (the `-e` option is for installing it in [development
mode](https://pip.pypa.io/en/latest/reference/pip_install.html#editable-installs)):

```sh
pip install -e .
```

See the full instructions for [installing from source](http://pandas.pydata.org/pandas-docs/stable/install.html#installing-from-source).

## License
BSD

## Documentation
The official documentation is hosted on PyData.org: http://pandas.pydata.org/pandas-docs/stable/

The Sphinx documentation should provide a good starting point for learning how
to use the library. Expect the docs to continue to expand as time goes on.

## Background
Work on ``pandas`` started at AQR (a quantitative hedge fund) in 2008 and
has been under active development since then.

## Getting Help

For usage questions, the best place to go to is [StackOverflow](https://stackoverflow.com/questions/tagged/pandas).
Further, general questions and discussions can also take place on the [pydata mailing list](https://groups.google.com/forum/?fromgroups#!forum/pydata).

## Discussion and Development
Most development discussion is taking place on github in this repo. Further, the [pandas-dev mailing list](https://mail.python.org/mailman/listinfo/pandas-dev) can also be used for specialized discussions or design issues, and a [Gitter channel](https://gitter.im/pydata/pandas) is available for quick development related questions.

## Contributing to pandas
All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.

A detailed overview on how to contribute can be found in the **[contributing guide.](http://pandas.pydata.org/pandas-docs/stable/contributing.html)**

If you are simply looking to start working with the pandas codebase, navigate to the [GitHub “issues” tab](https://github.com/pandas-dev/pandas/issues) and start looking through interesting issues. There are a number of issues listed under [Docs](https://github.com/pandas-dev/pandas/issues?labels=Docs&sort=updated&state=open) and [Difficulty Novice](https://github.com/pandas-dev/pandas/issues?q=is%3Aopen+is%3Aissue+label%3A%22Difficulty+Novice%22) where you could start out.

Or maybe through using pandas you have an idea of your own or are looking for something in the documentation and thinking ‘this can be improved’...you can do something about it!

Feel free to ask questions on the [mailing list](https://groups.google.com/forum/?fromgroups#!forum/pydata) or on [Gitter](https://gitter.im/pydata/pandas).
