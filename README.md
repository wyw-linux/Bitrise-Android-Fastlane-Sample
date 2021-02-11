# Bitrise Android Fastlane Sample

[![Bitrise status](https://app.bitrise.io/app/e6bc630bcb225bce/status.svg?token=wAXwQNEY8r-nqPD-XektbQ&branch=main)](https://app.bitrise.io/app/e6bc630bcb225bce)

This is a sample Android project that demonstrates a [Bitrise](https://bitrise.io) CI/CD setup using [Fastlane](https://fastlane.tools/). Build history is publicly available [here](https://app.bitrise.io/app/e6bc630bcb225bce#/builds).

## Project setup and config

This sample project is configured to run a Fastlane lane in Bitrise workflows. Lane `primary` does the following:

- Builds debug variant
- Runs lint and unit tests
- Copies lint and test reports to `$BITRISE_DEPLOY_DIR`, so you can access them as [artifacts](https://devcenter.bitrise.io/builds/build-artifacts-online/) on the build detail page

See [Fastfile](fastlane/Fastfile) for the full configuration.

For more complex Bitrise workflows, check out our other sample projects.

## Advanced use cases

While this repo demonstrates a simple project config on Bitrise, there are many advanced features that might be relevant for your project:

- [Generating multiple APKs (multi-flavor) in one workflow](https://devcenter.bitrise.io/deploy/android-deploy/generate-and-deploy-multiple-flavor-apks-in-a-single-workflow/)
- [Exporting a universal APK from an AAB](https://devcenter.bitrise.io/deploy/android-deploy/exporting-a-universal-apk-from-an-aab/)
- [Running tests in Visual Studio App Center](https://devcenter.bitrise.io/testing/run-your-tests-in-the-app-center/)
- [Measuring your code coverage with Codecov](https://devcenter.bitrise.io/testing/measuring-your-code-coverage-with-codecov/)
