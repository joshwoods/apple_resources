

- Core Media
-  CMSampleBufferGetOutputPresentationTimeStamp(\_:) 

Function

# CMSampleBufferGetOutputPresentationTimeStamp(\_:)

Returns the output presentation timestamp of a sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferGetOutputPresentationTimeStamp(_ sbuf: CMSampleBuffer) -> CMTime
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being interrogated.

## Return Value

The output presentation timestamp of the `CMSampleBuffer` or `kCMTimeInvalid` if there is an error.

## Discussion

The output presentation timestamp is the time at which the decoded, trimmed, stretched, and possibly reversed samples should start being presented. If CMSampleBufferGetOutputPresentationTimeStamp(_:) has been called to explicitly set the output PTS, CMSampleBufferGetOutputPresentationTimeStamp(_:) returns it. If not, CMSampleBufferGetOutputPresentationTimeStamp(_:) calculates its result as `(PresentationTimeStamp + TrimDurationAtStart)` unless `kCMSampleBufferAttachmentKey_Reverse` is `kCFBooleanTrue`, in which case it calculates the result as `(PresentationTimeStamp + Duration - TrimDurationAtEnd)`. These are generally correct for un-stretched, un-shifted playback.

For general forward playback in a scaled edit, the `OutputPresentationTimeStamp` should be set to:

`((PresentationTimeStamp + TrimDurationAtStart - EditStartMediaTime) / EditSpeedMultiplier) + EditStartTrackTime`

For general reversed playback:

`((PresentationTimeStamp + Duration - TrimDurationAtEnd - EditStartMediaTime) / EditSpeedMultiplier) + EditStartTrackTime`

## See Also

### Inspecting Duration and Timing

func CMSampleBufferGetDuration(CMSampleBuffer) -> CMTime

Returns the total duration of a sample buffer.

func CMSampleBufferGetDecodeTimeStamp(CMSampleBuffer) -> CMTime

Returns the decode timestamp that’s the earliest numerically of all the samples in a sample buffer.

func CMSampleBufferGetPresentationTimeStamp(CMSampleBuffer) -> CMTime

Returns the presentation timestamp that’s the earliest numerically of all the samples in a sample buffer.

func CMSampleBufferGetOutputDuration(CMSampleBuffer) -> CMTime

Returns the output duration of a sample buffer.

func CMSampleBufferGetOutputDecodeTimeStamp(CMSampleBuffer) -> CMTime

Returns the output decode timestamp of a sample buffer.

func CMSampleBufferSetOutputPresentationTimeStamp(CMSampleBuffer, newValue: CMTime) -> OSStatus

Sets an output presentation timestamp to use in place of a calculated value.

func CMSampleBufferGetSampleTimingInfo(CMSampleBuffer, at: CMItemIndex, timingInfoOut: UnsafeMutablePointer&lt;CMSampleTimingInfo>) -> OSStatus

Retrieves a timing information structure that describes a specified sample in a sample buffer.

func CMSampleBufferGetSampleTimingInfoArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;CMSampleTimingInfo>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of sample timing information structures that represents each sample in a sample buffer.

func CMSampleBufferGetOutputSampleTimingInfoArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;CMSampleTimingInfo>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of output timing information structures that represents each sample in a sample buffer.

