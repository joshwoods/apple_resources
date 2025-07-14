

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
- AnchoringComponent.Target.Alignment
-  init(\_:) 

Initializer

# init(\_:)

Creates a new set from a finite sequence of items.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

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

### Creating an alignment instance

init()

Creates an empty option set.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

init(rawValue: UInt8)

Creates a new option set from the given raw value.

