

- RealityKit
- AnimationFillMode
-  AnimationFillMode.RawValue 

Type Alias

# AnimationFillMode.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
typealias RawValue = Int8
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

## See Also

### Determining the element and raw value type

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

