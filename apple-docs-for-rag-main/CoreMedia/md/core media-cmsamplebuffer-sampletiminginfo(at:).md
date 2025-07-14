

- Core Media
- CMSampleBuffer
-  sampleTimingInfo(at:) 

Instance Method

# sampleTimingInfo(at:)

Returns sample timing information for a sample at the specified index.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func sampleTimingInfo(at sampleIndex: CMItemIndex) throws -> CMSampleTimingInfo
```

## Parameters 

`sampleIndex`  

The index of the sample to query for sample timing. The system raises an error if the sample index is out of range.

## Return Value

A structure that contains the decode and presentation timestamps of a sample.

## Discussion

The system throws a bufferHasNoSampleTimingInfo error if the buffer doesn’t contain sample timing.

## See Also

### Inspecting Duration and Timing

var duration: CMTime

The total duration of a sample buffer.

var decodeTimeStamp: CMTime

The decode timestamp of the first sample in the buffer.

var presentationTimeStamp: CMTime

The sample presentation timestamp that’s the earliest numerically in the sample buffer.

var outputDuration: CMTime

The output duration of the sample buffer.

var outputDecodeTimeStamp: CMTime

The output decode timestamp for a sample buffer.

var outputPresentationTimeStamp: CMTime

The output presentation timestamp of a sample buffer.

func setOutputPresentationTimeStamp(CMTime) throws

Sets an output presentation timestamp to use in place of a calculated value.

func sampleTimingInfos() throws -> [CMSampleTimingInfo]

Retrieves an array of sample timing information structures that represents each sample in a sample buffer.

func outputSampleTimingInfos() throws -> [CMSampleTimingInfo]

Retrieves an array of output sample timing information structures that represents each sample in a sample buffer.

