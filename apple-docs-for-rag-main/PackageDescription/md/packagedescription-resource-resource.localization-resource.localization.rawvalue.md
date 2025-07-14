

- PackageDescription
- Resource
- Resource.Localization
-  Resource.Localization.RawValue 

Type Alias

# Resource.Localization.RawValue

The raw type that can be used to represent all values of the conforming type.

SwiftPM 5.3+

``` source
typealias RawValue = String
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

## See Also

### Accessing the Raw Value

var rawValue: String

The corresponding value of the raw type.

