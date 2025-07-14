

- RealityKit
- ARView
- ARView.RenderOptions
-  ARView.RenderOptions.ArrayLiteralElement 

Type Alias

# ARView.RenderOptions.ArrayLiteralElement

The type of the elements of an array literal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
typealias ArrayLiteralElement = ARView.RenderOptions
```

## See Also

### Creating an option set

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

typealias Element

The element type of the option set.

init(rawValue: UInt)

Creates a new option set from the given raw value.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

let rawValue: UInt

The corresponding value of the raw type.

