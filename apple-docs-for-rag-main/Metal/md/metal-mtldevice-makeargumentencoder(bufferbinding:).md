

- Metal
- MTLDevice
-  makeArgumentEncoder(bufferBinding:) 

Instance Method

# makeArgumentEncoder(bufferBinding:)

Creates a new argument encoder for a buffer binding.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func makeArgumentEncoder(bufferBinding: any MTLBufferBinding) -> any MTLArgumentEncoder
```

**Required**

## Parameters 

`bufferBinding`  

An MTLBufferBinding instance.

## See Also

### Creating Argument Buffer Encoders

var argumentBuffersSupport: MTLArgumentBuffersTier

Returns the GPU device’s support tier for argument buffers.

**Required**

var maxArgumentBufferSamplerCount: Int

The maximum number of unique argument buffer samplers per app.

**Required**

func makeArgumentEncoder(arguments: [MTLArgumentDescriptor]) -> (any MTLArgumentEncoder)?

Creates a new argument encoder for an array of arguments.

**Required**

