

- Core Media
-  CMSampleBufferGetOutputDuration(\_:) 

Function

# CMSampleBufferGetOutputDuration(\_:)

Returns the output duration of a sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferGetOutputDuration(_ sbuf: CMSampleBuffer) -> CMTime
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being interrogated.

## Return Value

The output duration of the `CMSampleBuffer` or `kCMTimeInvalid` if there is an error.

## Discussion

The output duration is the duration minus any trimmed duration, all divided by the speed multiplier:

`(Duration - TrimDurationAtStart - TrimDurationAtEnd) / SpeedMultiplier`

## See Also

### Inspecting Duration and Timing

func CMSampleBufferGetDuration(CMSampleBuffer) -> CMTime

Returns the total duration of a sample buffer.

func CMSampleBufferGetDecodeTimeStamp(CMSampleBuffer) -> CMTime

Returns the decode timestamp that’s the earliest numerically of all the samples in a sample buffer.

func CMSampleBufferGetPresentationTimeStamp(CMSampleBuffer) -> CMTime

Returns the presentation timestamp that’s the earliest numerically of all the samples in a sample buffer.

func CMSampleBufferGetOutputDecodeTimeStamp(CMSampleBuffer) -> CMTime

Returns the output decode timestamp of a sample buffer.

func CMSampleBufferGetOutputPresentationTimeStamp(CMSampleBuffer) -> CMTime

Returns the output presentation timestamp of a sample buffer.

func CMSampleBufferSetOutputPresentationTimeStamp(CMSampleBuffer, newValue: CMTime) -> OSStatus

Sets an output presentation timestamp to use in place of a calculated value.

func CMSampleBufferGetSampleTimingInfo(CMSampleBuffer, at: CMItemIndex, timingInfoOut: UnsafeMutablePointer&lt;CMSampleTimingInfo>) -> OSStatus

Retrieves a timing information structure that describes a specified sample in a sample buffer.

func CMSampleBufferGetSampleTimingInfoArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;CMSampleTimingInfo>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of sample timing information structures that represents each sample in a sample buffer.

func CMSampleBufferGetOutputSampleTimingInfoArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;CMSampleTimingInfo>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of output timing information structures that represents each sample in a sample buffer.

