

- Metal
- MTLBlitCommandEncoder
-  resolveCounters(\_:range:destinationBuffer:destinationOffset:) 

Instance Method

# resolveCounters(\_:range:destinationBuffer:destinationOffset:)

Encodes a command that resolves the data from the samples in a sample counter buffer and stores the results into a buffer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOS

``` source
func resolveCounters(
    _ sampleBuffer: any MTLCounterSampleBuffer,
    range: Range,
    destinationBuffer: any MTLBuffer,
    destinationOffset: Int
)
```

## Parameters 

`sampleBuffer`  

A counter sample buffer source that contains the sample data.

`range`  

A range that indicates which of the buffer’s samples the command resolves.

`destinationBuffer`  

A destination buffer where the command stores the data it resolves.

`destinationOffset`  

A starting offset, in bytes, within `destinationBuffer` where the blit pass writes the first byte of the data it resolves.

## Mentioned in 

Converting a GPU’s Counter Data into a Readable Format

## Discussion

For an example of how and when to use this method, see Converting a GPU’s Counter Data into a Readable Format.

Note

The GPU stores MTLCounterErrorValue in `destinationBuffer` each time it encounters an error resolving a sample.

## See Also

### Working with Sample Counter Buffers

func sampleCounters(sampleBuffer: any MTLCounterSampleBuffer, sampleIndex: Int, barrier: Bool)

Encodes a command that samples the GPU’s hardware counters during a blit pass and stores the data in a counter sample buffer.

**Required**

