

- Swift Testing
- Trait
-  disabled(\_:sourceLocation:) 

Type Method

# disabled(\_:sourceLocation:)

Construct a condition trait that disables a test unconditionally.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
static func disabled(
    _ comment: Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation
) -> Self
```

Available when `Self` is `ConditionTrait`.

## Parameters 

`comment`  

An optional, user-specified comment describing this trait.

`sourceLocation`  

The source location of the trait.

## Return Value

An instance of ConditionTrait that will always disable the test to which it is added.

## Mentioned in 

Enabling and disabling tests

Organizing test functions with suite types

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

static func disabled(if: @autoclosure () throws -> Bool, Comment?, sourceLocation: SourceLocation) -> Self

Construct a condition trait that causes a test to be disabled if it returns `true`.

static func disabled(Comment?, sourceLocation: SourceLocation, () async throws -> Bool) -> Self

Construct a condition trait that causes a test to be disabled if it returns `true`.

static func timeLimit(TimeLimitTrait.Duration) -> Self

Construct a time limit trait that causes a test to time out if it runs for too long.

