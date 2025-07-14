

- RealityKit
- ARView
- ARView.EntityGestures
-  ARView.EntityGestures.Element 

Type Alias

# ARView.EntityGestures.Element

The element type of the option set.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
typealias Element = ARView.EntityGestures
```

## Discussion

To inherit all the default implementations from the `OptionSet` protocol, the `Element` type must be `Self`, the default.

## See Also

### Creating gesture option sets

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

typealias ArrayLiteralElement

The type of the elements of an array literal.

init(rawValue: Int)

Creates a new option set from the given raw value.

let rawValue: Int

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

