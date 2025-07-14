

- RealityKit
- LowLevelTexture
-  init(descriptor:) 

Initializer

# init(descriptor:)

Creates a low-level texture from a descriptor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
init(descriptor: LowLevelTexture.Descriptor) throws
```

## Parameters 

`descriptor`  

An object that defines the structure of the low-level texture.

## Discussion

Throws

If the descriptor is invalid or if memory was not allocated successfully.

