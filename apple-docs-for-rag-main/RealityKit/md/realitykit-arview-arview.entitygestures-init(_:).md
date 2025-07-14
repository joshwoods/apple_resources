

- RealityKit
- ARView
- ARView.EntityGestures
-  init(\_:) 

Initializer

# init(\_:)

Creates a new set from a finite sequence of items.

RealityKitSwiftiOSiPadOSMac Catalyst

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

### Creating gesture option sets

init()

Creates an empty option set.

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

