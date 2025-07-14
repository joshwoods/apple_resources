

- Metal
- MTLAccelerationStructurePassSampleBufferAttachmentDescriptor
-  sampleBuffer 

Instance Property

# sampleBuffer

A specialized memory buffer that the GPU uses to store its counter data during the acceleration structure pass.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var sampleBuffer: (any MTLCounterSampleBuffer)? { get set }
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Discussion

The property defaults to `nil`, which means the GPU doesn’t save any GPU counter information during the acceleration structure pass. See Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass and Sampling GPU Data into Counter Sample Buffers for more information.

