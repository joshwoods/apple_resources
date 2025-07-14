

- Metal
- MTLDevice
-  makeArgumentEncoder(arguments:) 

Instance Method

# makeArgumentEncoder(arguments:)

Creates a new argument encoder for an array of arguments.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func makeArgumentEncoder(arguments: [MTLArgumentDescriptor]) -> (any MTLArgumentEncoder)?
```

**Required**

## Parameters 

`arguments`  

An array of MTLArgumentDescriptor instances that you must sort by their index properties in monotonically increasing order.

## See Also

### Creating Argument Buffer Encoders

var argumentBuffersSupport: MTLArgumentBuffersTier

Returns the GPU device’s support tier for argument buffers.

**Required**

var maxArgumentBufferSamplerCount: Int

The maximum number of unique argument buffer samplers per app.

**Required**

func makeArgumentEncoder(bufferBinding: any MTLBufferBinding) -> any MTLArgumentEncoder

Creates a new argument encoder for a buffer binding.

**Required**

