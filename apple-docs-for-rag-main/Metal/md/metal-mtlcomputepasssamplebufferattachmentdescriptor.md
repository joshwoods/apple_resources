

- Metal
-  MTLComputePassSampleBufferAttachmentDescriptor 

Class

# MTLComputePassSampleBufferAttachmentDescriptor

A configuration that instructs the GPU where to store counter data from the beginning and end of a compute pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MTLComputePassSampleBufferAttachmentDescriptor
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Overview

For more context about configuring sample buffer attachments for compute passes, see Sampling GPU Data into Counter Sample Buffers. That article is one of a series in GPU Counters and Counter Sample Buffers about sampling Metal hardware counters for performance measurement.

## Topics

### Configuring the Sample Buffer Attachment

var sampleBuffer: (any MTLCounterSampleBuffer)?

A specialized memory buffer that the GPU uses to store its counter data during a compute pass.

var startOfEncoderSampleIndex: Int

An index within a counter sample buffer that tells the GPU where to store counter data from the start of a compute pass.

var endOfEncoderSampleIndex: Int

An index within a counter sample buffer that tells the GPU where to store counter data from the end of a compute pass.

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

class MTLComputePassDescriptor

A description of how to dispatch execution of pass commands and GPU performance sampling.

enum MTLDispatchType

The type of dispatch method to use when calling encoded functions.

struct MTLDispatchThreadgroupsIndirectArguments

The data layout required for arguments needed to specify the size of threadgroups.

class MTLComputePassSampleBufferAttachmentDescriptorArray

A container that stores an array of sample buffer attachments for a compute pass.

