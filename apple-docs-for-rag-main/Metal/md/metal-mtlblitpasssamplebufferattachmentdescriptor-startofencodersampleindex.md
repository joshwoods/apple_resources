

- Metal
- MTLBlitPassSampleBufferAttachmentDescriptor
-  startOfEncoderSampleIndex 

Instance Property

# startOfEncoderSampleIndex

An index within a counter sample buffer that tells the GPU where to store counter data from the start of a blit pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var startOfEncoderSampleIndex: Int { get set }
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Discussion

This property indicates where the GPU stores the counter data within an MTLCounterSampleBuffer instance that it samples at the beginning of a blit pass.

You can tell the GPU to skip sampling at the start of the blit pass by assigning MTLCounterDontSample to this property.

Important

For MTLDevice instances that don’t support MTLCounterSamplingPoint.atStageBoundary (see supportsCounterSampling(_:)), set this property to MTLCounterDontSample.

## See Also

### Configuring the Sample Buffer Attachment

var sampleBuffer: (any MTLCounterSampleBuffer)?

A specialized memory buffer that the GPU uses to store its counter data during the blit pass.

var endOfEncoderSampleIndex: Int

An index within a counter sample buffer that tells the GPU where to store counter data from the end of a blit pass.

