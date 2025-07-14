

- ARKit
- ARMatteGenerator
-  generateMatte(from:commandBuffer:) 

Instance Method

# generateMatte(from:commandBuffer:)

Generates alpha matte at either full resolution or half the resolution of the captured image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func generateMatte(
    from frame: ARFrame,
    commandBuffer: any MTLCommandBuffer
) -> any MTLTexture
```

## Return Value

An alpha matte texture at the resolution you chose at initialization.

