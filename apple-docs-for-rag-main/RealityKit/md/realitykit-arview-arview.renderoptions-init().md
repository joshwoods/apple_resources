

- RealityKit
- ARView
- ARView.RenderOptions
-  init() 

Initializer

# init()

Creates an empty option set.

RealityKitSwiftiOSiPadOSMac Catalyst

``` source
init()
```

Available when `RawValue` conforms to `FixedWidthInteger`.

## Discussion

This initializer creates an option set with a raw value of zero.

## See Also

### Creating an option set

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

typealias Element

The element type of the option set.

typealias ArrayLiteralElement

The type of the elements of an array literal.

init(rawValue: UInt)

Creates a new option set from the given raw value.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

let rawValue: UInt

The corresponding value of the raw type.

