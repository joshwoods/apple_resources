

- ARKit
- ARMatteGenerator
-  generateDilatedDepth(from:commandBuffer:) 

Instance Method

# generateDilatedDepth(from:commandBuffer:)

Generates dilated depth at the resolution of the segmentation stencil.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func generateDilatedDepth(
    from frame: ARFrame,
    commandBuffer: any MTLCommandBuffer
) -> any MTLTexture
```

## Return Value

A dilated depth texture which consists of a single channel of type `float32`.

## Discussion

You use the linear depth information this function provides when compositing a virtual object with the camera image.

