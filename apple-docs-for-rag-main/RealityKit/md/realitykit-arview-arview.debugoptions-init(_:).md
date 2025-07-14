

- RealityKit
- ARView
- ARView.DebugOptions
-  init(\_:) 

Initializer

# init(\_:)

Creates a new set from a finite sequence of items.

RealityKitSwiftiOSiPadOSMac CatalystmacOS

``` source
init(_ sequence: S) where S : Sequence, Self.Element == S.Element
```

## Parameters 

`sequence`  

The elements to use as members of the new set.

## Discussion

Use this initializer to create a new set from an existing sequence, like an array or a range:

```
let validIndices = Set(0..

## See Also

### Creating a debug option set

init()

Creates an empty option set.

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

