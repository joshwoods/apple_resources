

- Metal
- MTLComputePassDescriptor
-  sampleBufferAttachments 

Instance Property

# sampleBufferAttachments

The sample buffers that the compute pass can access.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var sampleBufferAttachments: MTLComputePassSampleBufferAttachmentDescriptorArray { get }
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Discussion

The GPU uses sample buffers to record performance information. See GPU Counters and Counter Sample Buffers, Sampling GPU Data into Counter Sample Buffers, and MTLCounter for more information.

