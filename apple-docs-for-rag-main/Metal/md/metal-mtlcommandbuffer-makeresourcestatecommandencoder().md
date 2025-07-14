

- Metal
- MTLCommandBuffer
-  makeResourceStateCommandEncoder() 

Instance Method

# makeResourceStateCommandEncoder()

Creates a resource state command encoder that uses default settings.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func makeResourceStateCommandEncoder() -> (any MTLResourceStateCommandEncoder)?
```

**Required**

## Discussion

Use an MTLResourceStateCommandEncoder instance’s methods to create a pass that updates the state of one or more sparse textures.

## See Also

### Creating Resource State Encoders

func resourceStateCommandEncoder(with: MTLResourceStatePassDescriptor) -> (any MTLResourceStateCommandEncoder)?

Creates a resource state command encoder from a descriptor.

**Required**

