

- Core Media
-  CMSampleBufferGetSampleTimingInfoArray(\_:entryCount:arrayToFill:entriesNeededOut:) 

Function

# CMSampleBufferGetSampleTimingInfoArray(\_:entryCount:arrayToFill:entriesNeededOut:)

Retrieves an array of sample timing information structures that represents each sample in a sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferGetSampleTimingInfoArray(
    _ sbuf: CMSampleBuffer,
    entryCount numSampleTimingEntries: CMItemCount,
    arrayToFill timingArrayOut: UnsafeMutablePointer?,
    entriesNeededOut timingArrayEntriesNeededOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being interrogated.

`numSampleTimingEntries`  

Number of entries in `timingArray`.\`\`

`timingArrayOut`  

On output, points to an array of `CMSampleTimingInfo` structs to receive the timing info.

`timingArrayEntriesNeededOut`  

Number of entries needed for the result.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

If only one `CMSampleTimingInfo` struct is returned, it applies to all samples in the buffer. See documentation of CMSampleTimingInfo for details of how a single `CMSampleTimingInfo` struct can apply to multiple samples.

The `timingArrayOut` must be allocated by the caller, and the number of entries allocated must be passed in `timingArrayEntries`. If `timingArrayOut` is `NULL`, `timingArrayEntriesNeededOut` will return the required number of entries. Similarly, if `timingArrayEntriesNeededOut` is too small, CMSampleBuffer will be returned, and `timingArrayEntriesNeededOut` will return the required number of entries. In either case, the caller can then make an appropriately-sized `timingArrayOut` and call again. For example, the caller might pass the address of a `CMSampleTimingInfo` struct on the stack (as `timingArrayOut`), and 1 as `timingArrayEntries`. If all samples are describable with a single `CMSampleTimingInfo` struct (or there’s only one sample in the `CMSampleBuffer`), this call will succeed. If not, it will fail, and will return the number of entries required in `timingArrayEntriesNeededOut`. Only in this case will the caller actually need to allocate an array. If there’s no `timingInfo` in this `CMSampleBuffer`, CMSampleBuffer will be returned, and `timingArrayEntriesNeededOut` will be set to 0.

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

func CMSampleBufferGetSampleTimingInfo(CMSampleBuffer, at: CMItemIndex, timingInfoOut: UnsafeMutablePointer&lt;CMSampleTimingInfo>) -> OSStatus

Retrieves a timing information structure that describes a specified sample in a sample buffer.

func CMSampleBufferGetOutputSampleTimingInfoArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;CMSampleTimingInfo>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of output timing information structures that represents each sample in a sample buffer.

