

- Metal
-  MTLPipelineOption 

Structure

# MTLPipelineOption

Options that determine how Metal prepares the pipeline.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
struct MTLPipelineOption
```

## Mentioned in 

Creating Binary Archives from Device-Built Pipeline State Objects

## Topics

### Retrieving Argument Information

static var bufferTypeInfo: MTLPipelineOption

An option instance that provides detailed buffer type information for buffer arguments.

static var failOnBinaryArchiveMiss: MTLPipelineOption

An option that specifies that Metal only creates the pipeline state object if the compiled shader is present inside a linked binary archive.

static var argumentInfo: MTLPipelineOption

An option instance that provides argument information for textures and threadgroup memory.

Deprecated

### Creating Compilation Options

init(rawValue: UInt)

Creates empty compilation options.

### Type Properties

static var bindingInfo: MTLPipelineOption

An option that provides binding information for pipeline state resources.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

class MTLPipelineBufferDescriptorArray

An array of pipeline buffer descriptors.

