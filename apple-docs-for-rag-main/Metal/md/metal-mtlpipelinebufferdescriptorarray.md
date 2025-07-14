

- Metal
-  MTLPipelineBufferDescriptorArray 

Class

# MTLPipelineBufferDescriptorArray

An array of pipeline buffer descriptors.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MTLPipelineBufferDescriptorArray
```

## Topics

### Accessing Array Elements

subscript(Int) -> MTLPipelineBufferDescriptor!

Returns the pipeline buffer descriptor at the specified array index.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Configuring a Compute Pipeline State

class MTLComputePipelineDescriptor

An instance describing the desired GPU state for a kernel call in a compute pass.

protocol MTLComputePipelineState

An interface that represents a GPU pipeline configuration for running kernels in a compute pass.

class MTLStageInputOutputDescriptor

A description of the input and output data of a function.

class MTLPipelineBufferDescriptor

The mutability options for a buffer that a render or compute pipeline uses.

struct MTLPipelineOption

Options that determine how Metal prepares the pipeline.

