

- Metal
- MTLRenderPassSampleBufferAttachmentDescriptor
-  startOfFragmentSampleIndex 

Instance Property

# startOfFragmentSampleIndex

The index the Metal device object should use to store GPU counters when starting the render pass’s fragment stage.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var startOfFragmentSampleIndex: Int { get set }
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

## Discussion

Specify MTLCounterDontSample if you don’t want to sample GPU counters at the start of the fragment stage. Otherwise, specify an index within the sample buffer where you want the GPU to write the sample data.

On devices that don’t support MTLCounterSamplingPoint.atStageBoundary you must set the value to MTLCounterDontSample.

## See Also

### Configuring the Sample Buffer Attachment

var sampleBuffer: (any MTLCounterSampleBuffer)?

A specialized memory buffer that the GPU uses to store its counter data during the render pass.

var startOfVertexSampleIndex: Int

The index the Metal device object should use to store GPU counters when starting the render pass’s vertex stage.

var endOfVertexSampleIndex: Int

The index the Metal device object should use to store GPU counters when ending the render pass’s vertex stage.

var endOfFragmentSampleIndex: Int

The index the Metal device object should use to store GPU counters when ending the render pass’s fragment stage.

