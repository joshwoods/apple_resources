

- Swift Testing
- ConditionTrait
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

