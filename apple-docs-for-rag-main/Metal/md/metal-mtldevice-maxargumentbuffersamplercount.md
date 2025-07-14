

- Metal
- MTLDevice
-  maxArgumentBufferSamplerCount 

Instance Property

# maxArgumentBufferSamplerCount

The maximum number of unique argument buffer samplers per app.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var maxArgumentBufferSamplerCount: Int { get }
```

**Required**

## Discussion

This limit only applies to samplers that support argument buffers (see supportArgumentBuffers). An MTLSamplerState instance is only unique if the properties of the MTLSamplerDescriptor instance that created it are unique. For example, two samplers with equal minFilter values but different magFilter values are unique.

See Improving CPU Performance by Using Argument Buffers for more information about argument buffer tiers, limits, and capabilities.

## See Also

### Creating Argument Buffer Encoders

var argumentBuffersSupport: MTLArgumentBuffersTier

Returns the GPU device’s support tier for argument buffers.

**Required**

func makeArgumentEncoder(arguments: [MTLArgumentDescriptor]) -> (any MTLArgumentEncoder)?

Creates a new argument encoder for an array of arguments.

**Required**

func makeArgumentEncoder(bufferBinding: any MTLBufferBinding) -> any MTLArgumentEncoder

Creates a new argument encoder for a buffer binding.

**Required**

