

- Metal
- MTLCommandBuffer
-  makeBlitCommandEncoder(descriptor:) 

Instance Method

# makeBlitCommandEncoder(descriptor:)

Creates a block information transfer (blit) encoder from a descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func makeBlitCommandEncoder(descriptor blitPassDescriptor: MTLBlitPassDescriptor) -> (any MTLBlitCommandEncoder)?
```

**Required**

## Parameters 

`blitPassDescriptor`  

An MTLBlitPassDescriptor instance that configures the MTLBlitCommandEncoder the method returns.

## Discussion

Use an MTLBlitCommandEncoder instance’s methods to create a block information transfer (blit) pass that quickly copies memory between a GPU device’s resources.

## See Also

### Creating Blit Encoders

func makeBlitCommandEncoder() -> (any MTLBlitCommandEncoder)?

Creates a block information transfer (blit) encoder.

**Required**

