

- Metal
- MTLResourceStatePassSampleBufferAttachmentDescriptor
-  startOfEncoderSampleIndex 

Instance Property

# startOfEncoderSampleIndex

The index the Metal device object should use to store GPU counters when starting the resource state pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var startOfEncoderSampleIndex: Int { get set }
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Discussion

Specify MTLCounterDontSample if you don’t want to sample GPU counters at the start of the resource state pass. Otherwise, specify an index within the sample buffer where you want the GPU to write the sample data.

On devices that don’t support MTLCounterSamplingPoint.atStageBoundary you must set the value to MTLCounterDontSample.

## See Also

### Configuring the Sample Buffer Attachment

var sampleBuffer: (any MTLCounterSampleBuffer)?

A specialized memory buffer that the GPU uses to store its counter data during the resource state pass.

var endOfEncoderSampleIndex: Int

The index the Metal device object should use to store GPU counters when ending the resource state pass.

