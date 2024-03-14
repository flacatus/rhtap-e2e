# Red Hat Trusted Application Pipeline Tests

> [!WARNING]  
> These tests are currently in a beta state.

The testing framework and End-to-End (E2E) tests for the Red Hat Trusted Application Pipeline are written in [Typescript](https://www.typescriptlang.org/) using the [Jest Framework](https://jestjs.io/).

## Features

- Instrumented tests with Jest. For more information, refer to the [Jest documentation](https://jestjs.io/docs).
- Ability to run E2E tests anywhere: locally (CRC/OpenShift local), OpenShift Cluster, OSD, etc.
- Writes test results in JUnit XML format to a custom directory. Set `JEST_JUNIT_OUTPUT_DIR=<artifacts-dir>` pointing to a valid directory. For example: `export JEST_JUNIT_OUTPUT_DIR="./artifacts"`.
- Customizable test suites with Jest globals.

## Getting Started

For installation instructions and how to run tests locally or in a CI environment, refer to the [Documentation](docs/Installation.md). This also contains information on pairing Pull Requests for introducing breaking changes.

## Development

For tips on developing new tests for RHTAP and guidelines on writing readable tests, refer to [Guidelines](docs/Guidelines.md).

## Debugging CI

To onboard a new component in Openshift CI or to debug CI jobs, follow the instructions in [OpenShift CI Documentation](docs/OpenShiftCI.md) and [Investigating CI Failures](docs/InvestigatingCIFailures.md), respectively.

**HAPPY TESTING!**
