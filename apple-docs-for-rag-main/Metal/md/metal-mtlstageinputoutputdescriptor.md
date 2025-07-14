

- Metal
-  MTLStageInputOutputDescriptor 

Class

# MTLStageInputOutputDescriptor

A description of the input and output data of a function.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class MTLStageInputOutputDescriptor
```

## Topics

### Describing Argument Layouts

var attributes: MTLAttributeDescriptorArray

An array that describes where and how to fetch data for the function.

var layouts: MTLBufferLayoutDescriptorArray

An array that describes how the function fetches data.

### Declaring Index Buffers for Indirect Compute Commands

var indexBufferIndex: Int

The location of the index buffer for a compute function using indexed thread addressing.

var indexType: MTLIndexType

The data type of the indices stored in the index buffer.

### Resetting the Descriptor

func reset()

Resets the default state for the descriptor.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configuring a Compute Pipeline State

class MTLComputePipelineDescriptor

An instance describing the desired GPU state for a kernel call in a compute pass.

protocol MTLComputePipelineState

An interface that represents a GPU pipeline configuration for running kernels in a compute pass.

class MTLPipelineBufferDescriptor

The mutability options for a buffer that a render or compute pipeline uses.

class MTLPipelineBufferDescriptorArray

An array of pipeline buffer descriptors.

struct MTLPipelineOption

Options that determine how Metal prepares the pipeline.

