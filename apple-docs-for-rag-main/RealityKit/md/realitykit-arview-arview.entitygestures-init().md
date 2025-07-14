

- RealityKit
- ARView
- ARView.EntityGestures
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

### Creating gesture option sets

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

typealias Element

The element type of the option set.

typealias ArrayLiteralElement

The type of the elements of an array literal.

init(rawValue: Int)

Creates a new option set from the given raw value.

let rawValue: Int

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

