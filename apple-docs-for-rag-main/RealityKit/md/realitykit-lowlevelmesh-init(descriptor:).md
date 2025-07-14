

- RealityKit
- LowLevelMesh
-  init(descriptor:) 

Initializer

# init(descriptor:)

Constructs a low-level mesh from a descriptor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
init(descriptor: LowLevelMesh.Descriptor) throws
```

## Parameters 

`descriptor`  

An object that defines the structure of the low-level mesh.

## Discussion

Throws

If the descriptor is invalid or if you do not successfully allocate its memory.

