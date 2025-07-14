

- Core Media
- CMSampleBuffer
-  sampleSize(at:) 

Instance Method

# sampleSize(at:)

Returns the size of a sample in bytes.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func sampleSize(at sampleIndex: Int) -> Int
```

## Parameters 

`sampleIndex`  

The index of the sample to query.

## Return Value

The size of the sample.

## Discussion

If you specify a sample index that isn’t in the range, the system returns `0`. It also returns `0` if the sample buffer contains no sizes, which occurs if the samples in the buffer are noncontiguous, such as noninterleaved audio, or if the sample buffer contains a CVImageBuffer.

## See Also

### Inspecting Size Information

var numSamples: Int

The number of media samples the buffer contains.

func sampleSizes() throws -> [Int]

Retrieves an array of sample sizes that represents each sample in a sample buffer.

var totalSampleSize: Int

The total size in bytes of sample data in the buffer.

