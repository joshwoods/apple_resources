

- RealityKit
- ARView
- ARView.DebugOptions
-  init() 

Initializer

# init()

Creates an empty option set.

RealityKitSwiftiOSiPadOSMac CatalystmacOS

``` source
init()
```

Available when `RawValue` conforms to `FixedWidthInteger`.

## Discussion

This initializer creates an option set with a raw value of zero.

## See Also

### Creating a debug option set

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

typealias Element

The element type of the option set.

typealias ArrayLiteralElement

The type of the elements of an array literal.

init(rawValue: Int)

Create a debug options enumeration from a raw value.

let rawValue: Int

Options for drawing overlay content in a scene that aids in debugging the scene.

