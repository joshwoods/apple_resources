

- Video Toolbox
-  VTDecompressionOutputCallback 

Type Alias

# VTDecompressionOutputCallback

The prototype for the callback invoked when frame decompression is complete.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
typealias VTDecompressionOutputCallback = (UnsafeMutableRawPointer?, UnsafeMutableRawPointer?, OSStatus, VTDecodeInfoFlags, CVImageBuffer?, CMTime, CMTime) -> Void
```

## Parameters 

`decompressionOutputRefCon`  

The callback’s reference value, copied from the `decompressionOutputRefCon` field of the VTDecompressionOutputCallbackRecord structure.

`sourceFrameRefCon`  

The frame’s reference value, copied from the `sourceFrameRefCon` argument to `VTDecompressionSessionDecodeFrame`.

`status`  

`noErr` if decompression was successful; an error code if decompression was not successful.

`infoFlags`  

Information about the decode operation.

The asynchronous bit may be set if the decode ran asynchronously.

The frameDropped bit may be set if the frame was dropped.

If the imageBufferModifiable bit is set, it is safe for the client to modify the imageBuffer.

`imageBuffer`  

The decompressed frame, if decompression was successful; otherwise, `NULL`.

Important

The video decompressor may still be referencing the `imageBuffer` returned in this callback if the imageBufferModifiable flag is not set. Unless this flag is set, it is not safe to modify the returned `imageBuffer`.

`presentationTimeStamp`  

The frame’s presentation timestamp, which is determined by calling CMSampleBufferGetOutputPresentationTimeStamp(_:); otherwise, `kCMTimeInvalid` if the timestamp is not available.

`presentationDuration`  

The frame’s presentation duration, which is determined by calling CMSampleBufferGetOutputDuration(_:); otherwise, `kCMTimeInvalid` if the timestamp is not available.

## Discussion

When you create a decompression session, you pass in a callback function to be called for decompressed frames. This function is not necessarily called in display order.

## See Also

### Data Types

class VTDecompressionSession

A reference to a decompression session.

struct VTDecodeFrameFlags

Flags to pass to a decompression session and the video decoder.

struct VTDecodeInfoFlags

Flags that provide information about the status of a decode operation.

struct VTDecompressionOutputCallbackRecord

typealias VTDecompressionOutputHandler

The prototype for the block invoked when frame decompression is complete.

