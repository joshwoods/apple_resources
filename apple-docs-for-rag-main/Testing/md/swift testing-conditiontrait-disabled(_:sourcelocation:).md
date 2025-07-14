

- Swift Testing
- ConditionTrait
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

