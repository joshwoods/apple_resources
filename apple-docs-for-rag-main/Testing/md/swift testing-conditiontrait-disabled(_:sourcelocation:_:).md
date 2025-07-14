

- Swift Testing
- ConditionTrait
-  disabled(\_:sourceLocation:\_:) 

Type Method

# disabled(\_:sourceLocation:\_:)

Construct a condition trait that causes a test to be disabled if it returns `true`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
static func disabled(
    _ comment: Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation,
    _ condition: @escaping () async throws -> Bool
) -> Self
```

Available when `Self` is `ConditionTrait`.

## Parameters 

`comment`  

An optional, user-specified comment describing this trait.

`sourceLocation`  

The source location of the trait.

`condition`  

A closure containing the trait’s custom condition logic. If this closure returns `false`, the test is allowed to run. Otherwise, the test is skipped.

## Return Value

An instance of ConditionTrait that will evaluate the specified closure.

