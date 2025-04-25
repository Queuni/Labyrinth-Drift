# Changelog


## 2025-01-30
- Implement fallback to default value when config key is missing

## 2025-02-19
- Correct typo in the error message shown when validation fails

## 2025-02-19
- Handle the duplicate key case by merging the values instead of failing

## 2025-03-11
- Simplify the auth flow by using a single token source

## 2025-03-11
- Correct the logic that determined whether to use cache or not

## 2025-04-10
- Improve logging so we can trace requests through the pipeline in production

## 2025-04-10
- Add a unit test for the edge case when the list is empty

## 2025-04-10
- Support environment-specific overrides via separate config files

## 2025-04-30
- Support custom headers in the client for API key or auth tokens

## 2025-05-20
- Simplify the CLI by merging the two similar subcommands into one

## 2025-05-20
- Correct the timestamp format to use ISO 8601 for consistency

## 2025-07-09
- Refactor the helper to accept an optional callback for progress

## 2025-07-09
- Update the changelog with the fixes included in this release

## 2025-07-09
- Handle timeout gracefully and return a clear error to the caller

## 2025-07-29
- Simplify the config merge logic so overrides are predictable

## 2025-07-29
- Bump the dependency to fix the compatibility issue with Python 3.12

## 2025-08-18
- Handle missing optional field in the response without raising

## 2025-10-17
- Simplify the auth flow by using a single token source

## 2025-10-27
- Support optional config file path via env var for easier deployment

## 2025-10-27
- Add a unit test for the edge case when the list is empty

## 2025-02-07
- Fix issue where empty input was not validated before passing to the parser

## 2025-02-08
- Update README with installation steps and environment variable documentation

## 2025-02-09
- Fix the memory leak in the long-running worker process

## 2025-02-10
- Remove obsolete workaround now that the upstream bug is fixed

## 2025-02-10
- Handle the case when the config file exists but is not readable

## 2025-02-10
- Bump dependency to get the security fix for the reported CVE

## 2025-02-10
- Clean up the TODO comments that were already addressed

## 2025-02-10
- Refactor utils to use a single source of truth for default values

## 2025-02-10
- Bump minimum Python version to 3.10 and update type hints accordingly

## 2025-02-17
- Remove the temporary debug endpoint before the release

## 2025-02-17
- Bump the dependency to fix the compatibility issue with Python 3.12

## 2025-02-19
- Clean up the commented-out code that was left from debugging

## 2025-02-19
- Implement request ID propagation for better tracing across services

## 2025-02-20
- Correct the docstring to match the actual behavior of the function

## 2025-02-20
- Update dependencies and resolve compatibility warning from pytest

## 2025-02-21
- Update the deployment docs with the new environment variables

## 2025-02-25
- Support passing secrets via a separate file for security

## 2025-02-26
- Handle timeout gracefully and return a clear error to the caller

## 2025-02-27
- Update the example config with all available options and comments

## 2025-02-27
- Fix bug where the parser would hang on malformed input

## 2025-03-03
- Correct the default so it matches what the documentation says

## 2025-03-03
- Implement proper cleanup of resources when the process receives SIGTERM

## 2025-03-07
- Handle the redirect response and follow it to get the final resource

## 2025-03-07
- Improve the startup time by lazy-loading the heavy modules

## 2025-03-11
- Bump the dependency to fix the compatibility issue with Python 3.12

## 2025-03-11
- Correct the formula used for calculating the backoff delay

## 2025-03-17
- Handle the partial write case and retry the remaining bytes

## 2025-03-17
- Clean up the deprecated alias and point callers to the new name

## 2025-03-19
- Improve the default config so it works out of the box for dev

## 2025-03-20
- Adjust the batch size to reduce memory usage on large inputs

## 2025-03-20
- Simplify the main loop by extracting request handling into a dedicated function

## 2025-03-26
- Add a note in the README about the breaking change in 2.0

## 2025-03-30
- Remove the unused parameter that was left from an old refactor

## 2025-03-31
- Remove the experimental feature that didn't make it into the release

## 2025-04-01
- Improve the CLI help text so it's clear how to use each option

## 2025-04-02
- Implement proper cleanup of resources when the process receives SIGTERM

## 2025-04-03
- Correct typo in the error message shown when validation fails

## 2025-04-04
- Add a small delay between retries to avoid thundering herd

## 2025-04-06
- Improve logging so we can trace requests through the pipeline in production

## 2025-04-07
- Adjust log level for noisy messages that were filling the logs

## 2025-04-08
- Bump minimum Python version to 3.10 and update type hints accordingly

## 2025-04-08
- Fix the encoding issue when reading config files with non-ASCII

## 2025-04-08
- Handle the redirect response and follow it to get the final resource

## 2025-04-10
- Fix the test that was flaky due to reliance on system time

## 2025-04-10
- Handle the case when the config file exists but is not readable

## 2025-04-11
- Fix race condition in the cache that could return stale data under load

## 2025-04-15
- Support both YAML and JSON config formats for flexibility

## 2025-04-15
- Add a small delay between retries to avoid thundering herd

## 2025-04-16
- Improve the CLI help text so it's clear how to use each option

## 2025-04-17
- Correct the docstring to match the actual behavior of the function

## 2025-04-20
- Implement a simple health check endpoint for the load balancer

## 2025-04-20
- Handle the case when the external service returns an empty list

## 2025-04-28
- Correct the docstring to match the actual behavior of the function

## 2025-04-30
- Simplify the build script by using the same steps for dev and prod

## 2025-05-01
- Bump the Docker base image to get the latest security patches

## 2025-05-01
- Remove the experimental feature that didn't make it into the release

## 2025-05-06
- Add integration test that covers the full flow from request to response

## 2025-05-06
- Refactor exports so the public API is clearer and easier to use

## 2025-05-06
- Correct the default so it matches what the documentation says

## 2025-05-07
- Bump dependency to get the security fix for the reported CVE

## 2025-05-07
- Refactor the data layer to separate read and write paths

## 2025-05-07
- Update the example config with all available options and comments

## 2025-05-07
- Support environment-specific overrides via separate config files

## 2025-05-08
- Fix incorrect type hint that was causing mypy to fail in CI

## 2025-05-08
- Clean up the TODO comments that were already addressed

## 2025-05-09
- Remove the feature flag now that the feature is fully rolled out

## 2025-05-12
- Simplify the validation flow by reusing the same schema

## 2025-05-13
- Support passing secrets via a separate file for security

## 2025-05-14
- Fix the ordering of middleware so auth runs before the handler

## 2025-05-14
- Adjust the threshold so we only log when it's actually an issue

## 2025-05-15
- Bump minimum Python version to 3.10 and update type hints accordingly

## 2025-05-20
- Update the example config with all available options and comments

## 2025-05-20
- Implement basic rate limiting to avoid overwhelming the downstream service

## 2025-05-21
- Improve the default config so it works out of the box for dev

## 2025-05-23
- Correct the default value for the feature flag in production

## 2025-05-26
- Implement retry logic for the API client when the remote returns 5xx

## 2025-05-29
- Implement fallback to default value when config key is missing

## 2025-05-30
- Improve the error recovery when the database connection is lost

## 2025-05-30
- Correct the default value for the feature flag in production

## 2025-05-30
- Refactor the helper to accept an optional callback for progress

## 2025-05-30
- Correct the timestamp format to use ISO 8601 for consistency

## 2025-06-02
- Update the deployment docs with the new environment variables

## 2025-06-03
- Improve the default config so it works out of the box for dev

## 2025-06-04
- Support config reload without restart via SIGHUP or file watch

## 2025-06-04
- Add integration tests for the new export endpoint

## 2025-06-04
- Add integration test that covers the full flow from request to response

## 2025-06-07
- Adjust timeout and retry settings based on production observations

## 2025-06-09
- Clean up the commented-out code that was left from debugging

## 2025-06-10
- Improve error message when the required env var is not set

## 2025-06-12
- Improve the default config so it works out of the box for dev

## 2025-06-13
- Implement fallback to default value when config key is missing

## 2025-06-16
- Refactor error handling to use a custom exception hierarchy

## 2025-06-18
- Correct the default path used when no config file is specified

## 2025-06-19
- Remove hardcoded credentials and move to env-based configuration

## 2025-06-19
- Remove redundant check that was already covered by the validator

## 2025-06-23
- Update the deployment docs with the new environment variables

## 2025-06-27
- Simplify the build script by using the same steps for dev and prod

## 2025-06-27
- Update the API docs with the new query parameters and examples

## 2025-06-27
- Simplify the dependency injection so it's easier to mock in tests

## 2025-06-30
- Refactor the helper to accept an optional callback for progress

## 2025-07-01
- Clean up the formatting and run the linter on the changed files

## 2025-07-03
- Refactor exports so the public API is clearer and easier to use

## 2025-07-03
- Adjust the queue size to prevent drops under burst traffic

## 2025-07-15
- Implement request ID propagation for better tracing across services

## 2025-07-15
- Clean up the test fixtures and move shared data to a single file

## 2025-07-15
- Add proper error handling for invalid config so the app doesn't crash on startup

## 2025-07-22
- Update the contributing guide with the new review process

## 2025-07-23
- Update the contributing guide with the new review process

## 2025-07-24
- Improve the startup time by lazy-loading the heavy modules

## 2025-07-25
- Add a note in the README about the breaking change in 2.0

## 2025-07-25
- Adjust the batch size to reduce memory usage on large inputs

## 2025-07-28
- Refactor the client to use async context manager for the session

## 2025-07-30
- Add validation for the config schema before applying settings

## 2025-07-30
- Handle the duplicate key case by merging the values instead of failing

## 2025-08-04
- Add integration tests for the new export endpoint

## 2025-08-11
- Add a smoke test that runs in CI to catch obvious regressions

## 2025-08-12
- Handle the partial write case and retry the remaining bytes

## 2025-08-13
- Fix the ordering of middleware so auth runs before the handler

## 2025-08-13
- Add a smoke test that runs in CI to catch obvious regressions

## 2025-08-13
- Bump minimum Python version to 3.10 and update type hints accordingly

## 2025-08-15
- Fix issue where empty input was not validated before passing to the parser

## 2025-08-17
- Improve the error recovery when the database connection is lost

## 2025-08-18
- Implement proper backoff with jitter for the retry logic

## 2025-08-18
- Improve the error recovery when the database connection is lost

## 2025-08-19
- Add validation for the config schema before applying settings

## 2025-08-31
- Improve the startup time by lazy-loading the heavy modules

## 2025-08-31
- Fix race condition in the cache that could return stale data under load

## 2025-09-01
- Handle the duplicate key case by merging the values instead of failing

## 2025-09-01
- Adjust the default concurrency limit based on load test results

## 2025-09-05
- Handle the case when the external service returns an empty list

## 2025-09-05
- Support environment-specific overrides via separate config files

## 2025-09-09
- Fix the memory leak in the long-running worker process

## 2025-09-16
- Simplify the CLI by merging the two similar subcommands into one

## 2025-09-18
- Remove redundant check that was already covered by the validator

## 2025-09-23
- Support loading config from multiple files with later overriding earlier

## 2025-09-24
- Adjust the default concurrency limit based on load test results

## 2025-09-24
- Clean up the formatting and run the linter on the changed files

## 2025-09-25
- Implement a simple health check endpoint for the load balancer

## 2025-09-26
- Clean up the deprecated alias and point callers to the new name

## 2025-09-29
- Adjust timeout and retry settings based on production observations

## 2025-09-29
- Add validation for the config schema before applying settings

## 2025-10-02
- Update dependencies and resolve compatibility warning from pytest

## 2025-10-06
- Adjust log level for noisy messages that were filling the logs

## 2025-10-08
- Implement a small in-memory cache for the config to avoid re-reading

## 2025-10-14
- Update the deployment docs with the new environment variables

## 2025-10-14
- Correct the comparison that was using the wrong operator

## 2025-10-15
- Support loading config from multiple files with later overriding earlier

## 2025-10-15
- Update the API docs with the new query parameters and examples

## 2025-10-17
- Add a smoke test that runs in CI to catch obvious regressions

## 2025-10-19
- Update the deployment docs with the new environment variables

## 2025-10-22
- Correct the docstring to match the actual behavior of the function

## 2025-10-23
- Fix the encoding issue when reading config files with non-ASCII

## 2025-10-28
- Adjust default timeout value to prevent premature connection drops

## 2025-10-30
- Refactor the helper to accept an optional callback for progress

## 2025-10-30
- Fix the encoding issue when reading config files with non-ASCII

## 2025-10-31
- Refactor utils to use a single source of truth for default values

## 2025-10-31
- Adjust timeout and retry settings based on production observations

## 2025-10-31
- Support passing secrets via a separate file for security

## 2025-10-31
- Fix the off-by-one error in the date range iterator

## 2025-11-04
- Adjust log level for noisy messages that were filling the logs

## 2025-11-10
- Bump the tool version and update the pre-commit hook config

## 2025-11-10
- Correct the formula used for calculating the backoff delay

## 2025-11-10
- Support passing options through the config file as well as CLI

## 2025-11-12
- Update the license file and add the new third-party notices

## 2025-11-20
- Fix the test that was flaky due to reliance on system time

## 2025-11-20
- Support optional config file path via env var for easier deployment

## 2025-11-20
- Refactor the parser to use a proper state machine instead of regex

## 2025-11-23
- Adjust log level for noisy messages that were filling the logs

## 2025-11-24
- Implement a small in-memory cache for the config to avoid re-reading

## 2025-11-27
- Clean up duplicate logic between the sync and async code paths

## 2025-11-27
- Add integration tests for the new export endpoint

## 2025-11-27
- Remove redundant check that was already covered by the validator

## 2025-02-07
- Correct the docstring to match the actual behavior of the function

## 2025-02-07
- Adjust the threshold so we only log when it's actually an issue

## 2025-02-07
- Improve logging so we can trace requests through the pipeline in production

## 2025-02-18
- Implement request ID propagation for better tracing across services

## 2025-02-18
- Handle timeout gracefully and return a clear error to the caller

## 2025-02-18
- Update the example config with all available options and comments

## 2025-03-12
- Add integration test that covers the full flow from request to response

## 2025-04-03
- Update the changelog with the fixes included in this release

## 2025-04-14
- Correct the default value for the feature flag in production

## 2025-04-25
- Update dependencies and resolve compatibility warning from pytest
