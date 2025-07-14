

- Video Toolbox
-  VTCompressionSessionBeginPass(\_:flags:\_:) 

Function

# VTCompressionSessionBeginPass(\_:flags:\_:)

Marks the start of a specific compression pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
func VTCompressionSessionBeginPass(
    _ session: VTCompressionSession,
    flags beginPassFlags: VTCompressionSessionOptionFlags,
    _ reserved: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`session`  

A compression session.

`beginPassFlags`  

Pass beginFinalPass to inform the encoder that the pass must be the final pass.

`reserved`  

A reserved value.

## Discussion

During multipass encoding, this function must be called before VTCompressionSessionEncodeFrame(_:imageBuffer:presentationTimeStamp:duration:frameProperties:sourceFrameRefcon:infoFlagsOut:).

It’s an error to call this function when multipass encoding is not enabled by setting kVTCompressionPropertyKey_MultiPassStorage.

## Topics

### Option Flags

struct VTCompressionSessionOptionFlags

Flags to pass to a compression session.

## See Also

### Performing Multiple Passes

func VTCompressionSessionEndPass(VTCompressionSession, furtherPassesRequestedOut: UnsafeMutablePointer&lt;DarwinBoolean>?, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

Marks the end of a compression pass.

func VTCompressionSessionGetTimeRangesForNextPass(VTCompressionSession, timeRangeCountOut: UnsafeMutablePointer&lt;CMItemCount>, timeRangeArrayOut: UnsafeMutablePointer&lt;UnsafePointer&lt;CMTimeRange>?>) -> OSStatus

Retrieves the time ranges for the next pass.

