

- Metal
-  MTLDispatchType 

Enumeration

# MTLDispatchType

The type of dispatch method to use when calling encoded functions.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
enum MTLDispatchType
```

## Topics

### Execution Dispatch Types

case concurrent

Sets a command encoder to dispatch encoded commands concurrently during your pass.

case serial

Sets a command encoder to dispatch encoded commands serially during your pass.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring a Compute Pass

class MTLComputePassDescriptor

A description of how to dispatch execution of pass commands and GPU performance sampling.

struct MTLDispatchThreadgroupsIndirectArguments

The data layout required for arguments needed to specify the size of threadgroups.

class MTLComputePassSampleBufferAttachmentDescriptor

A configuration that instructs the GPU where to store counter data from the beginning and end of a compute pass.

class MTLComputePassSampleBufferAttachmentDescriptorArray

A container that stores an array of sample buffer attachments for a compute pass.

