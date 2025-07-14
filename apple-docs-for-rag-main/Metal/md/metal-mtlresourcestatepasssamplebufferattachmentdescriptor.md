

- Metal
-  MTLResourceStatePassSampleBufferAttachmentDescriptor 

Class

# MTLResourceStatePassSampleBufferAttachmentDescriptor

A description of where to store GPU counter information at the start and end of a resource state pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLResourceStatePassSampleBufferAttachmentDescriptor
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Topics

### Configuring the Sample Buffer Attachment

var sampleBuffer: (any MTLCounterSampleBuffer)?

A specialized memory buffer that the GPU uses to store its counter data during the resource state pass.

var startOfEncoderSampleIndex: Int

The index the Metal device object should use to store GPU counters when starting the resource state pass.

var endOfEncoderSampleIndex: Int

The index the Metal device object should use to store GPU counters when ending the resource state pass.

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

### Sparse Textures

Managing Sparse Texture Memory

Take direct control of memory allocation for texture data by using sparse textures.

Creating Sparse Heaps and Sparse Textures

Allocate memory for sparse textures by creating a sparse heap.

Converting Between Pixel Regions and Sparse Tile Regions

Learn how a sparse texture’s contents are organized in memory.

Assigning Memory to Sparse Textures

Use a resource state encoder to allocate and deallocate sparse tiles for a sparse texture.

Reading and Writing to Sparse Textures

Decide how to handle access to unmapped texture regions.

Estimating How Often a Texture Region Is Accessed

Use texture access patterns to determine when you need to map a texture region.

class MTLResourceStatePassDescriptor

A configuration for a resource state pass, used to create a resource state command encoder.

class MTLResourceStatePassSampleBufferAttachmentDescriptorArray

An array of sample buffer attachments for a resource state pass.

protocol MTLResourceStateCommandEncoder

An encoder that encodes commands that modify resource configurations.

struct MTLMapIndirectArguments

The data layout for mapping sparse texture regions when using indirect commands.

