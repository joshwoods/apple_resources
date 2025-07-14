

- Video Toolbox
-  VTCompressionSessionGetTimeRangesForNextPass(\_:timeRangeCountOut:timeRangeArrayOut:) 

Function

# VTCompressionSessionGetTimeRangesForNextPass(\_:timeRangeCountOut:timeRangeArrayOut:)

Retrieves the time ranges for the next pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
func VTCompressionSessionGetTimeRangesForNextPass(
    _ session: VTCompressionSession,
    timeRangeCountOut: UnsafeMutablePointer,
    timeRangeArrayOut: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`session`  

The compression session.

`timeRangeCountOut`  

A pointer to the item count (CMItemCount) to receive the number of `CMTimeRanges`.

`timeRangeArrayOut`  

A pointer to a C array of `CMTimeRanges`. The storage for this array belongs to the compression session and should not be modified.The pointer is valid until the next call to VTCompressionSessionEndPass(_:furtherPassesRequestedOut:_:), or until the compression session is invalidated or finalized.

## Discussion

If VTCompressionSessionEndPass(_:furtherPassesRequestedOut:_:) sets `furtherPassesRequestedOut` to true, call this function to find out the time ranges for the next pass. Source frames outside these time ranges should be skipped. Each time range includes any frame at its start time and does not include any frame at its end time.

It’s an error to call this function when multipass encoding has not been enabled by setting kVTCompressionPropertyKey_MultiPassStorage, or when `VTCompressionSessionEndPass` did not set f`urtherPassesRequestedOut` to true.

## See Also

### Performing Multiple Passes

func VTCompressionSessionBeginPass(VTCompressionSession, flags: VTCompressionSessionOptionFlags, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

Marks the start of a specific compression pass.

func VTCompressionSessionEndPass(VTCompressionSession, furtherPassesRequestedOut: UnsafeMutablePointer&lt;DarwinBoolean>?, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

Marks the end of a compression pass.

