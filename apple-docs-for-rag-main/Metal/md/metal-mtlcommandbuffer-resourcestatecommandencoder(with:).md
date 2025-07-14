

- Metal
- MTLCommandBuffer
-  resourceStateCommandEncoder(with:) 

Instance Method

# resourceStateCommandEncoder(with:)

Creates a resource state command encoder from a descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func resourceStateCommandEncoder(with resourceStatePassDescriptor: MTLResourceStatePassDescriptor) -> (any MTLResourceStateCommandEncoder)?
```

**Required**

## Parameters 

`resourceStatePassDescriptor`  

An MTLResourceStatePassDescriptor instance that configures the MTLResourceStateCommandEncoder the method returns.

## Discussion

Use an MTLResourceStateCommandEncoder instance’s methods to create a pass that updates the state of one or more sparse textures.

## See Also

### Creating Resource State Encoders

func makeResourceStateCommandEncoder() -> (any MTLResourceStateCommandEncoder)?

Creates a resource state command encoder that uses default settings.

**Required**

