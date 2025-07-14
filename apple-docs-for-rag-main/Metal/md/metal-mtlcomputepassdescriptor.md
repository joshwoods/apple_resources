

- Metal
-  MTLComputePassDescriptor 

Class

# MTLComputePassDescriptor

A description of how to dispatch execution of pass commands and GPU performance sampling.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MTLComputePassDescriptor
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Topics

### Configuring the Dispatch Mechanism

var dispatchType: MTLDispatchType

The strategy for dispatching any compute commands encoded in the compute pass.

### Specifying Sample Buffers for GPU Counters

var sampleBufferAttachments: MTLComputePassSampleBufferAttachmentDescriptorArray

The sample buffers that the compute pass can access.

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

### Configuring a Compute Pass

enum MTLDispatchType

The type of dispatch method to use when calling encoded functions.

struct MTLDispatchThreadgroupsIndirectArguments

The data layout required for arguments needed to specify the size of threadgroups.

class MTLComputePassSampleBufferAttachmentDescriptor

A configuration that instructs the GPU where to store counter data from the beginning and end of a compute pass.

class MTLComputePassSampleBufferAttachmentDescriptorArray

A container that stores an array of sample buffer attachments for a compute pass.

