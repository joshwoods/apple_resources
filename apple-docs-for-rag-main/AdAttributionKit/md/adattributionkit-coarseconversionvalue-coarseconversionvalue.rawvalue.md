

- AdAttributionKit
- CoarseConversionValue
-  CoarseConversionValue.RawValue 

Type Alias

# CoarseConversionValue.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 17.4+iPadOS 17.4+Mac Catalyst

``` source
typealias RawValue = String
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

