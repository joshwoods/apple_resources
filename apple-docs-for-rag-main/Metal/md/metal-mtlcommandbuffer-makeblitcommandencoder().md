

- Metal
- MTLCommandBuffer
-  makeBlitCommandEncoder() 

Instance Method

# makeBlitCommandEncoder()

Creates a block information transfer (blit) encoder.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeBlitCommandEncoder() -> (any MTLBlitCommandEncoder)?
```

**Required**

## Discussion

Use an MTLBlitCommandEncoder instance’s methods to create a block information transfer (blit) pass that quickly copies memory between a GPU device’s resources.

## See Also

### Creating Blit Encoders

func makeBlitCommandEncoder(descriptor: MTLBlitPassDescriptor) -> (any MTLBlitCommandEncoder)?

Creates a block information transfer (blit) encoder from a descriptor.

**Required**

