

- Core Media
- CMSampleBuffer
-  decodeTimeStamp 

Instance Property

# decodeTimeStamp

The decode timestamp of the first sample in the buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var decodeTimeStamp: CMTime { get }
```

## Discussion

The system expects sample buffers to store samples in their decode order, even if their presentation order is different.

This value is invalid if there’s an error.

## See Also

### Inspecting Duration and Timing

var duration: CMTime

The total duration of a sample buffer.

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

func sampleTimingInfo(at: CMItemIndex) throws -> CMSampleTimingInfo

Returns sample timing information for a sample at the specified index.

func outputSampleTimingInfos() throws -> [CMSampleTimingInfo]

Retrieves an array of output sample timing information structures that represents each sample in a sample buffer.

