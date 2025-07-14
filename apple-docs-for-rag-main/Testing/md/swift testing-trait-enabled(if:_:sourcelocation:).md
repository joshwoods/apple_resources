

- Swift Testing
- Trait
-  enabled(if:\_:sourceLocation:) 

Type Method

# enabled(if:\_:sourceLocation:)

Construct a condition trait that causes a test to be disabled if it returns `false`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
static func enabled(
    if condition: @autoclosure @escaping () throws -> Bool,
    _ comment: Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation
) -> Self
```

Available when `Self` is `ConditionTrait`.

## Parameters 

`condition`  

A closure containing the trait’s custom condition logic. If this closure returns `true`, the test is allowed to run. Otherwise, the test is skipped.

`comment`  

An optional, user-specified comment describing this trait.

`sourceLocation`  

The source location of the trait.

## Return Value

An instance of ConditionTrait that will evaluate the specified closure.

## Mentioned in 

Enabling and disabling tests

## See Also

### Customizing runtime behaviors

Enabling and disabling tests

Conditionally enable or disable individual tests before they run.

Limiting the running time of tests

Set limits on how long a test can run for until it fails.

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

