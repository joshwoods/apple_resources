

- Video Toolbox
-  VTCompressionSessionEndPass(\_:furtherPassesRequestedOut:\_:) 

Function

# VTCompressionSessionEndPass(\_:furtherPassesRequestedOut:\_:)

Marks the end of a compression pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
func VTCompressionSessionEndPass(
    _ session: VTCompressionSession,
    furtherPassesRequestedOut: UnsafeMutablePointer?,
    _ reserved: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`session`  

The compression session.

`furtherPassesRequestedOut`  

A pointer to a Boolean that is set to true if the video encoder requests to perform another pass, false otherwise. You may pass `NULL` to indicate that the client is certain to use this as the final pass, in which case the video encoder can skip that evaluation step.

`reserved`  

Reserved for future use and not currently used. Pass `NULL` for this argument.

## Discussion

This function can take a long time, because the video encoder may perform significant processing between passes. You indicate with the `furtherPassesRequestedOut` argument whether the video encoder is requesting another pass. There is no particular limit on the number of passes the video encoder may request, but the client is free to disregard this request and use the last-emitted set of frames.

It’s an error to call this function when multi-pass encoding has not been enabled by setting kVTCompressionPropertyKey_MultiPassStorage.

## See Also

### Performing Multiple Passes

func VTCompressionSessionBeginPass(VTCompressionSession, flags: VTCompressionSessionOptionFlags, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

Marks the start of a specific compression pass.

func VTCompressionSessionGetTimeRangesForNextPass(VTCompressionSession, timeRangeCountOut: UnsafeMutablePointer&lt;CMItemCount>, timeRangeArrayOut: UnsafeMutablePointer&lt;UnsafePointer&lt;CMTimeRange>?>) -> OSStatus

Retrieves the time ranges for the next pass.

