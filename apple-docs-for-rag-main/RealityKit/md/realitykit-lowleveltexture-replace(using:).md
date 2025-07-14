

- RealityKit
- LowLevelTexture
-  replace(using:) 

Instance Method

# replace(using:)

Retrieves a Metal texture that your app’s shaders can write to when they run on a GPU.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
func replace(using commandBuffer: any MTLCommandBuffer) -> any MTLTexture
```

## Parameters 

`commandBuffer`  

The MTLCommandBuffer you intend to use for texture modifications. RealityKit waits for the command buffer to complete before utilizing the texture for rendering.

## Discussion

The buffer’s contents are in an uninitialized state.

