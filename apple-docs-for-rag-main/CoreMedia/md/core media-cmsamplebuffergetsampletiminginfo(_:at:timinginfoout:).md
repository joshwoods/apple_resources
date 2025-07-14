

- Core Media
-  CMSampleBufferGetSampleTimingInfo(\_:at:timingInfoOut:) 

Function

# CMSampleBufferGetSampleTimingInfo(\_:at:timingInfoOut:)

Retrieves a timing information structure that describes a specified sample in a sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferGetSampleTimingInfo(
    _ sbuf: CMSampleBuffer,
    at sampleIndex: CMItemIndex,
    timingInfoOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being interrogated.

`sampleIndex`  

Sample index (0 is the first sample in `sbuf`).

`timingInfoOut`  

On output, points to a single `CMSampleTimingInfo` struct to receive the timing info.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

A sample-specific CMSampleTimingInfo struct will be returned with a sample-specific `presentationTimeStamp` and `decodeTimeStamp`, even if a single `CMSampleTimingInfo` struct was used during creation to describe all the samples in the buffer. The timing info struct must be allocated by the caller. If the sample index isn’t in the range 0…numSamples-1, CMSampleBuffer will be returned. If there’s no `timingInfo` in this `CMSampleBuffer`, CMSampleBuffer will be returned.

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

func CMSampleBufferGetOutputPresentationTimeStamp(CMSampleBuffer) -> CMTime

Returns the output presentation timestamp of a sample buffer.

func CMSampleBufferSetOutputPresentationTimeStamp(CMSampleBuffer, newValue: CMTime) -> OSStatus

Sets an output presentation timestamp to use in place of a calculated value.

func CMSampleBufferGetSampleTimingInfoArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;CMSampleTimingInfo>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of sample timing information structures that represents each sample in a sample buffer.

func CMSampleBufferGetOutputSampleTimingInfoArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;CMSampleTimingInfo>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of output timing information structures that represents each sample in a sample buffer.

