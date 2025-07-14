

- Metal
- MTLResourceStatePassSampleBufferAttachmentDescriptor
-  sampleBuffer 

Instance Property

# sampleBuffer

A specialized memory buffer that the GPU uses to store its counter data during the resource state pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var sampleBuffer: (any MTLCounterSampleBuffer)? { get set }
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Discussion

The property defaults to `nil`, which means the GPU doesn’t save any GPU counter information during the resource state pass. See Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass and Sampling GPU Data into Counter Sample Buffers for more information.

## See Also

### Configuring the Sample Buffer Attachment

var startOfEncoderSampleIndex: Int

The index the Metal device object should use to store GPU counters when starting the resource state pass.

var endOfEncoderSampleIndex: Int

The index the Metal device object should use to store GPU counters when ending the resource state pass.

