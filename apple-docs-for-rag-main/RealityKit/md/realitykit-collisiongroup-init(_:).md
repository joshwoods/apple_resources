

- RealityKit
- CollisionGroup
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

### Creating a collision group

init()

Creates an empty option set.

init(rawValue: UInt32)

Creates a collision group from a raw value.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

