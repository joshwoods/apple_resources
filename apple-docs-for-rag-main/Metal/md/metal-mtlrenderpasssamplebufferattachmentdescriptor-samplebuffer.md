

- Metal
- MTLRenderPassSampleBufferAttachmentDescriptor
-  sampleBuffer 

Instance Property

# sampleBuffer

A specialized memory buffer that the GPU uses to store its counter data during the render pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var sampleBuffer: (any MTLCounterSampleBuffer)? { get set }
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Discussion

The property defaults to `nil`, which means the GPU doesn’t save any GPU counter information during the render pass. See Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass and Sampling GPU Data into Counter Sample Buffers for more information.

## See Also

### Configuring the Sample Buffer Attachment

var startOfVertexSampleIndex: Int

The index the Metal device object should use to store GPU counters when starting the render pass’s vertex stage.

var endOfVertexSampleIndex: Int

The index the Metal device object should use to store GPU counters when ending the render pass’s vertex stage.

var startOfFragmentSampleIndex: Int

The index the Metal device object should use to store GPU counters when starting the render pass’s fragment stage.

var endOfFragmentSampleIndex: Int

The index the Metal device object should use to store GPU counters when ending the render pass’s fragment stage.

