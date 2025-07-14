

- Swift Testing
- Trait
-  timeLimit(\_:) 

Type Method

# timeLimit(\_:)

Construct a time limit trait that causes a test to time out if it runs for too long.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+Swift 6.0+Xcode 16.0+

``` source
static func timeLimit(_ timeLimit: TimeLimitTrait.Duration) -> Self
```

Available when `Self` is `TimeLimitTrait`.

## Parameters 

`timeLimit`  

The maximum amount of time the test may run for.

## Return Value

An instance of TimeLimitTrait.

## Mentioned in 

Limiting the running time of tests

## Discussion

Test timeouts do not support high-precision, arbitrarily short durations due to variability in testing environments. The time limit must be at least one minute, and can only be expressed in increments of one minute.

When this trait is associated with a test, that test must complete within a time limit of, at most, `timeLimit`. If the test runs longer, an issue of kind Issue.Kind.timeLimitExceeded(timeLimitComponents:) is recorded. This timeout is treated as a test failure.

The time limit amount specified by `timeLimit` may be reduced if the testing library is configured to enforce a maximum per-test limit. When such a maximum is set, the effective time limit of the test this trait is applied to will be the lesser of `timeLimit` and that maximum. This is a policy which may be configured on a global basis by the tool responsible for launching the test process. Refer to that tool’s documentation for more details.

If a test is parameterized, this time limit is applied to each of its test cases individually. If a test has more than one time limit associated with it, the shortest one is used. A test run may also be configured with a maximum time limit per test case.

## See Also

### Customizing runtime behaviors

Enabling and disabling tests

Conditionally enable or disable individual tests before they run.

Limiting the running time of tests

Set limits on how long a test can run for until it fails.

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

