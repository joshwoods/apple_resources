

- Video Toolbox
-  VTCompressionOutputCallback 

Type Alias

# VTCompressionOutputCallback

A callback for the system to invoke when it’s finished compressing a frame.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
typealias VTCompressionOutputCallback = (UnsafeMutableRawPointer?, UnsafeMutableRawPointer?, OSStatus, VTEncodeInfoFlags, CMSampleBuffer?) -> Void
```

## Parameters 

`outputCallbackRefCon`  

The callback’s reference value.

`sourceFrameRefCon`  

The frame’s reference value, copied from the `sourceFrameRefCon` argument to VTCompressionSessionEncodeFrame(_:imageBuffer:presentationTimeStamp:duration:frameProperties:sourceFrameRefcon:infoFlagsOut:).

`status`  

`noErr` if compression was successful; an error code if compression wasn’t successful.

`infoFlags`  

Contains information about the encode operation.

The asynchronous bit may be set if the encode ran asynchronously.

The frameDropped bit may be set if the frame was dropped.

`sampleBuffer`  

Contains the compressed frame if compression was successful and the frame wasn’t dropped; otherwise, `NULL`.

## Discussion

When you create a compression session, you pass in a callback function to be called for compressed frames. This function is called in decode order (which is not necessarily the same as display order).

## See Also

### Callbacks

typealias VTCompressionOutputHandler

A callback for the system to invoke when it’s finished compressing a frame.

