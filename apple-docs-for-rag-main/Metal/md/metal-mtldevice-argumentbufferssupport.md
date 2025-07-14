

- Metal
- MTLDevice
-  argumentBuffersSupport 

Instance Property

# argumentBuffersSupport

Returns the GPU device’s support tier for argument buffers.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var argumentBuffersSupport: MTLArgumentBuffersTier { get }
```

**Required**

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

## Topics

### Argument Buffer Tiers

enum MTLArgumentBuffersTier

The values that determine the limits and capabilities of argument buffers.

## See Also

### Creating Argument Buffer Encoders

var maxArgumentBufferSamplerCount: Int

The maximum number of unique argument buffer samplers per app.

**Required**

func makeArgumentEncoder(arguments: [MTLArgumentDescriptor]) -> (any MTLArgumentEncoder)?

Creates a new argument encoder for an array of arguments.

**Required**

func makeArgumentEncoder(bufferBinding: any MTLBufferBinding) -> any MTLArgumentEncoder

Creates a new argument encoder for a buffer binding.

**Required**

