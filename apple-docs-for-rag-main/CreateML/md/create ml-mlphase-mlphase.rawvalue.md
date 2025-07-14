

- Create ML
- MLPhase
-  MLPhase.RawValue 

Type Alias

# MLPhase.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
typealias RawValue = String
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

## See Also

### Getting a phase’s string value

var rawValue: String

The corresponding value of the raw type.

