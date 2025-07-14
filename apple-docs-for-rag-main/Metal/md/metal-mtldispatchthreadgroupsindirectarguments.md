

- Metal
-  MTLDispatchThreadgroupsIndirectArguments 

Structure

# MTLDispatchThreadgroupsIndirectArguments

The data layout required for arguments needed to specify the size of threadgroups.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLDispatchThreadgroupsIndirectArguments
```

## Mentioned in 

Specifying Drawing and Dispatch Arguments Indirectly

## Topics

### Specifying the Size of the Threadgroup

init()

Returns a new data layout for dispatching threadgroups over indirect buffer calls.

init(threadgroupsPerGrid: (UInt32, UInt32, UInt32))

Returns a new data layout for dispatching threadgroups over indirect buffer calls, with specified threadgroups per grid.

var threadgroupsPerGrid: (UInt32, UInt32, UInt32)

The number of threadgroups for the grid, in each dimension.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Related Documentation

func dispatchThreadgroups(indirectBuffer: any MTLBuffer, indirectBufferOffset: Int, threadsPerThreadgroup: MTLSize)

Encodes a dispatch call for a compute pass, using an indirect buffer that defines the size of a grid that aligns to threadgroup boundaries.

**Required**

### Configuring a Compute Pass

class MTLComputePassDescriptor

A description of how to dispatch execution of pass commands and GPU performance sampling.

enum MTLDispatchType

The type of dispatch method to use when calling encoded functions.

class MTLComputePassSampleBufferAttachmentDescriptor

A configuration that instructs the GPU where to store counter data from the beginning and end of a compute pass.

class MTLComputePassSampleBufferAttachmentDescriptorArray

A container that stores an array of sample buffer attachments for a compute pass.

