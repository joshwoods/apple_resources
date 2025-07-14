

- Metal
- MTLComputeCommandEncoder
-  sampleCounters(sampleBuffer:sampleIndex:barrier:) 

Instance Method

# sampleCounters(sampleBuffer:sampleIndex:barrier:)

Encodes a command to sample hardware counters, providing performance information.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func sampleCounters(
    sampleBuffer: any MTLCounterSampleBuffer,
    sampleIndex: Int,
    barrier: Bool
)
```

**Required**

## Parameters 

`sampleBuffer`  

An MTLCounterSampleBuffer instance that stores the GPU hardware data.

`sampleIndex`  

An index within `sampleBuffer` the command stores the data to.

`barrier`  

Whether or not the command inserts a barrier before sampling the counter’s data.

A barrier ensures that the commands you encode before this one complete before the GPU samples the hardware counters, but can negatively impact runtime performance.

Running this command without a barrier means the GPU can sample counters concurrently with other commands from the encoder.

The `barrier` parameter for the command has no impact on sampling commands from other passes.

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Discussion

Important

To use a sample buffer, it must be part of the sampleBufferAttachments on the compute pass descriptor.

See GPU Counters and Counter Sample Buffers, Sampling GPU Data into Counter Sample Buffers, and MTLCounter for more information.

