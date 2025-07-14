

- Metal
-  MTLComputePassSampleBufferAttachmentDescriptorArray 

Class

# MTLComputePassSampleBufferAttachmentDescriptorArray

A container that stores an array of sample buffer attachments for a compute pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MTLComputePassSampleBufferAttachmentDescriptorArray
```

## Overview

The number of elements in the array is at least the number of elements in an MTLDevice instance’s counterSets property.

## Topics

### Accessing a Sample Buffer Attachment

subscript(Int) -> MTLComputePassSampleBufferAttachmentDescriptor!

Returns the descriptor object for the specified sample buffer attachment.

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

### Configuring a Compute Pass

class MTLComputePassDescriptor

A description of how to dispatch execution of pass commands and GPU performance sampling.

enum MTLDispatchType

The type of dispatch method to use when calling encoded functions.

struct MTLDispatchThreadgroupsIndirectArguments

The data layout required for arguments needed to specify the size of threadgroups.

class MTLComputePassSampleBufferAttachmentDescriptor

A configuration that instructs the GPU where to store counter data from the beginning and end of a compute pass.

