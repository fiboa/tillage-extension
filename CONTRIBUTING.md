# Contributing

All contributions are subject to the
[Code of Conduct](https://vecorel.org/code-of-conduct/).

## Running tests

You'll need to install Python >= 3.9 and pip to setup the test environment.
We use pipenv to execute the tests.

Start with the following command in the folder where this README is located:
`pip install pipenv --user`

Install the dependencies for the test:
`pipenv install`

Finally, you can run the tests as follows:

- To check the markdown run: `pipenv run test-docs`
- To check the schema run: `pipenv run test-schema`
- To check the examples run: `pipenv run test-examples`
- To create a GeoParquet from the GeoJSON examples: `pipenv run create-geoparquet`
