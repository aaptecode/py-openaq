[![Build Status](https://travis-ci.org/dhhagan/py-openaq.svg?branch=master)](https://travis-ci.org/dhhagan/py-openaq)
[![PyPI version](https://badge.fury.io/py/py-openaq.svg)](https://badge.fury.io/py/py-openaq)
[![Coverage Status](https://coveralls.io/repos/dhhagan/py-openaq/badge.svg?branch=master&service=github)](https://coveralls.io/github/dhhagan/py-openaq?branch=master)

# py-openaq
This project contains the python wrapper for the [Open AQ API][1].

Full documentation can be found [here][2]!



## Installation

    pip install py-openaq

## Contributing to Development

### Generating Documentation

Documentation is generated using [sphinx][3] and [auto-doc][4]. Please see their respective documents for help.
Docs are automatically built for each new release, but you can build them locally using the following command
 from within the `/docs` directory:

    make html

### Suggesting Enhancements

If there is a feature you would like to see added, please submit as an [Issue][5].
Feel free to send pull requests if you are comfortable, otherwise another developer will try to reply to any issue requests.

### Running Tests Locally

To run the tests locally:

    python setup.py test

To run the tests locally with coverage:

    coverage run --source openaq setup.py test

    # View the report
    coverage report -m

## Quickstart

    import openaq

    api = openaq.OpenAQ()

    status, resp = api.cities()


[1]: https://docs.openaq.org/
[2]: http://py-openaq.readthedocs.org/en/latest/
[3]: http://www.sphinx-doc.org/en/stable/
[4]: http://www.sphinx-doc.org/en/stable/ext/autodoc.html
[5]: https://github.com/dhhagan/py-openaq/issues/new
