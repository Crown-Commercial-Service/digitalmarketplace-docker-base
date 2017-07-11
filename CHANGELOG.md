# Digital Marketplace base Docker image

Records breaking changes from major version bumps

## 2.0.0

PR: [#13](https://github.com/alphagov/digitalmarketplace-docker-base/pull/13)

### What changed?

The base image is now created from a Python 3 base image. This means that apps will run on Python 3. Python 3 versions are being run with a separate VERSION file and base docker image, as we will need to run Python 2 and Python 3 apps while we make the transition, starting with the API.

Having a separate VERSION file (PY2VERSION for Python 2) will allow us to build a push docker images for both versions simultaneously.

## 1.0.0

Initial version.
