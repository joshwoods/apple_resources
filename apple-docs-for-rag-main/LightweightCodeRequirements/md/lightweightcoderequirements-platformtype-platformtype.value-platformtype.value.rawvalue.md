

- LightweightCodeRequirements
- PlatformType
- PlatformType.Value
-  PlatformType.Value.RawValue 

Type Alias

# PlatformType.Value.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
typealias RawValue = Int64
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

