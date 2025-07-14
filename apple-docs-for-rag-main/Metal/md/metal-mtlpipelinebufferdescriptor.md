

- Metal
-  MTLPipelineBufferDescriptor 

Class

# MTLPipelineBufferDescriptor

The mutability options for a buffer that a render or compute pipeline uses.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MTLPipelineBufferDescriptor
```

## Overview

Metal can perform additional optimizations if you guarantee that neither the CPU nor the GPU modify a buffer’s contents before starting a pass. Use immutable buffers as much as possible to take advantage of Metal optimizations.

To declare that a buffer is immutable, set the mutability property of their associated MTLPipelineBufferDescriptor object to MTLMutability.immutable.

## Topics

### Setting Buffer Mutability

var mutability: MTLMutability

A mutability option that determines whether you can update a buffer’s contents before related commands use the buffer.

enum MTLMutability

The options that determine the mutability of a buffer’s contents.

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

class MTLStageInputOutputDescriptor

A description of the input and output data of a function.

class MTLPipelineBufferDescriptorArray

An array of pipeline buffer descriptors.

struct MTLPipelineOption

Options that determine how Metal prepares the pipeline.

