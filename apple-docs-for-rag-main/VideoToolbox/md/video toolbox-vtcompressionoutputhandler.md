

- Video Toolbox
-  VTCompressionOutputHandler 

Type Alias

# VTCompressionOutputHandler

A callback for the system to invoke when it’s finished compressing a frame.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 10.2+visionOS 1.0+

``` source
typealias VTCompressionOutputHandler = (OSStatus, VTEncodeInfoFlags, CMSampleBuffer?) -> Void
```

## Parameters 

`status`  

`noErr` if compression was successful; an error code if compression was not successful.

`infoFlags`  

Contains information about the encode operation.

The asynchronous bit may be set if the encode ran asynchronously.

The frameDropped bit may be set if the frame was dropped.

`sampleBuffer`  

Contains the compressed frame if compression was successful and the frame was not dropped; otherwise, `NULL`.

## Discussion

When you encode a frame, you pass in a callback block to be called for that compressed frame. This block is called in decode order (which is not necessarily the same as display order).

## See Also

### Callbacks

typealias VTCompressionOutputCallback

A callback for the system to invoke when it’s finished compressing a frame.

