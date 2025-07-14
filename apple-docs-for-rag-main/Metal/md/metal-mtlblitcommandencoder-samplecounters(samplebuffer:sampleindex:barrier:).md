

- Metal
- MTLBlitCommandEncoder
-  sampleCounters(sampleBuffer:sampleIndex:barrier:) 

Instance Method

# sampleCounters(sampleBuffer:sampleIndex:barrier:)

Encodes a command that samples the GPU’s hardware counters during a blit pass and stores the data in a counter sample buffer.

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

A counter sample buffer where the command stores the sample data.

`sampleIndex`  

A location within `sampleBuffer` where the command stores the sample data.

`barrier`  

A Boolean value that indicates whether the command inserts a barrier before taking the sample.

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Discussion

Inserting a barrier ensures that any work you encode with this encoder is complete before the GPU samples the hardware counters. If you don’t insert a barrier, the GPU can sample the counters concurrently with other commands you encode with this encoder. Using a barrier can help the counter results be more predictable and repeatable, but it may adversely affect your app’s runtime performance.

Note

The GPU doesn’t isolate this sampling command from any commands that come from another encoder, with or without a barrier.

## See Also

### Working with Sample Counter Buffers

func resolveCounters(any MTLCounterSampleBuffer, range: Range&lt;Int>, destinationBuffer: any MTLBuffer, destinationOffset: Int)

Encodes a command that resolves the data from the samples in a sample counter buffer and stores the results into a buffer.

