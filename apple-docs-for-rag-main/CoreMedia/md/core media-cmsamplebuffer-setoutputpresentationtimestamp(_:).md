

- Core Media
- CMSampleBuffer
-  setOutputPresentationTimeStamp(\_:) 

Instance Method

# setOutputPresentationTimeStamp(\_:)

Sets an output presentation timestamp to use in place of a calculated value.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setOutputPresentationTimeStamp(_ pts: CMTime) throws
```

## Parameters 

`pts`  

The output presentation timestamp.

## Discussion

This value is the time at which the system should present the decoded, trimmed, stretched and possibly reversed samples. By default, retrieving the value of the `outputPresentationTimeStamp` property calculates the time dynamically. You can use this method to set a specific value for `outputPresentationTimeStamp`.

For general forward playback in a scaled edit, calculate the timestamp as follows:

`((PresentationTimeStamp + TrimDurationAtStart - EditStartMediaTime) / EditSpeedMultiplier) + EditStartTrackTime`

For general reversed playback, calculate the timestamp as shown below:

`((PresentationTimeStamp + Duration - TrimDurationAtEnd - EditStartMediaTime) / EditSpeedMultiplier) + EditStartTrackTime`

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

func sampleTimingInfos() throws -> [CMSampleTimingInfo]

Retrieves an array of sample timing information structures that represents each sample in a sample buffer.

func sampleTimingInfo(at: CMItemIndex) throws -> CMSampleTimingInfo

Returns sample timing information for a sample at the specified index.

func outputSampleTimingInfos() throws -> [CMSampleTimingInfo]

Retrieves an array of output sample timing information structures that represents each sample in a sample buffer.

