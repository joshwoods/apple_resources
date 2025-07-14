

- RealityKit
- ARView
- 
  - ARView
- ARView.Environment
- ARView.Environment.SceneUnderstanding
- ARView.Environment.SceneUnderstanding.Options
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

