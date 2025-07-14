

- Metal
-  MTLCounterDontSample 

Global Variable

# MTLCounterDontSample

A sentinel value that instructs an encoder to skip sampling a counter as the GPU runs the encoder’s pass.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var MTLCounterDontSample: Int { get }
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Discussion

You can skip sampling at specific stages by assigning this sentinel value to the following properties instead of an offset to a counter sample buffer:

| Types | Properties |
|----|----|
| MTLRenderPassSampleBufferAttachmentDescriptor | startOfVertexSampleIndex  endOfVertexSampleIndex  startOfFragmentSampleIndex  endOfFragmentSampleIndex |
| MTLComputePassSampleBufferAttachmentDescriptor | startOfEncoderSampleIndex  endOfEncoderSampleIndex |
| MTLBlitPassSampleBufferAttachmentDescriptor | startOfEncoderSampleIndex  endOfEncoderSampleIndex |
| MTLResourceStatePassSampleBufferAttachmentDescriptor | startOfEncoderSampleIndex  endOfEncoderSampleIndex |
| MTLAccelerationStructurePassSampleBufferAttachmentDescriptor | startOfEncoderSampleIndex  endOfEncoderSampleIndex |

## See Also

### Counter Sample Buffers

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

Make a buffer that provides a place for a GPU to save its runtime performance metrics as it runs a pass.

class MTLCounterSampleBufferDescriptor

A group of properties that configures the counter sample buffers you create with it.

protocol MTLCounterSampleBuffer

A specialized memory buffer that stores a GPU’s counter set data.

Sampling GPU Data into Counter Sample Buffers

Retrieve a GPU’s counter data at a time the GPU supports.

