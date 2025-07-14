

- Swift Testing
- Traits
-  Limiting the running time of tests 

Article

# Limiting the running time of tests

Set limits on how long a test can run for until it fails.

## Overview

Some tests may naturally run slowly: they may require significant system resources to complete, may rely on downloaded data from a server, or may otherwise be dependent on external factors.

If a test may hang indefinitely or may consume too many system resources to complete effectively, consider setting a time limit for it so that it’s marked as failing if it runs for an excessive amount of time. Use the timeLimit(_:) trait as an upper bound:

```
@Test(.timeLimit(.minutes(60))
func serve100CustomersInOneHour() async {
  for _ in 0 ..

If the above test function takes longer than an hour (60 x 60 seconds) to execute, the task in which it’s running is cancelled and the test fails with an issue of kind Issue.Kind.timeLimitExceeded(timeLimitComponents:).

Note

If multiple time limit traits apply to a test, the shortest time limit is used.

The testing library may adjust the specified time limit for performance reasons or to ensure tests have enough time to run. In particular, a granularity of (by default) one minute is applied to tests. The testing library can also be configured with a maximum time limit per test that overrides any applied time limit traits.

### Time limits applied to test suites

When a time limit is applied to a test suite, it’s recursively applied to all test functions and child test suites within that suite.

### Time limits applied to parameterized tests

When a time limit is applied to a parameterized test function, it’s applied to each invocation *separately* so that if only some arguments cause failures, then successful arguments aren’t incorrectly marked as failing too.

## See Also

### Customizing runtime behaviors

Enabling and disabling tests

Conditionally enable or disable individual tests before they run.

static func enabled(if: @autoclosure () throws -> Bool, Comment?, sourceLocation: SourceLocation) -> Self

Construct a condition trait that causes a test to be disabled if it returns `false`.

static func enabled(Comment?, sourceLocation: SourceLocation, () async throws -> Bool) -> Self

Construct a condition trait that causes a test to be disabled if it returns `false`.

static func disabled(Comment?, sourceLocation: SourceLocation) -> Self

Construct a condition trait that disables a test unconditionally.

static func disabled(if: @autoclosure () throws -> Bool, Comment?, sourceLocation: SourceLocation) -> Self

Construct a condition trait that causes a test to be disabled if it returns `true`.

static func disabled(Comment?, sourceLocation: SourceLocation, () async throws -> Bool) -> Self

Construct a condition trait that causes a test to be disabled if it returns `true`.

static func timeLimit(TimeLimitTrait.Duration) -> Self

Construct a time limit trait that causes a test to time out if it runs for too long.

