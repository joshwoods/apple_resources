

- Video Toolbox
-  VTCompressionSessionEncodeFrame(\_:imageBuffer:presentationTimeStamp:duration:frameProperties:sourceFrameRefcon:infoFlagsOut:) 

Function

# VTCompressionSessionEncodeFrame(\_:imageBuffer:presentationTimeStamp:duration:frameProperties:sourceFrameRefcon:infoFlagsOut:)

Presents frames to the compression session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTCompressionSessionEncodeFrame(
    _ session: VTCompressionSession,
    imageBuffer: CVImageBuffer,
    presentationTimeStamp: CMTime,
    duration: CMTime,
    frameProperties: CFDictionary?,
    sourceFrameRefcon: UnsafeMutableRawPointer?,
    infoFlagsOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`session`  

The compression session.

`imageBuffer`  

A Core Video image buffer (CVImageBuffer) containing a video frame to be compressed. The buffer must have a nonzero reference count.

`presentationTimeStamp`  

The presentation timestamp for this frame, to be attached to the sample buffer. Each presentation timestamp passed to a session must be greater than the previous one.

`duration`  

The presentation duration for this frame, to be attached to the sample buffer. If you do not have duration information, pass invalid.

`frameProperties`  

Key/value pairs specifying additional properties for encoding this frame. Note that some session properties may also be changed between frames. Such changes affect subsequently encoded frames.

`sourceFrameRefcon`  

Your reference value for the frame, which will be passed to the output callback function.

`infoFlagsOut`  

A pointer to a `VTEncodeInfoFlags` to receive information about the encode operation.

The asynchronous bit may be set if the encode is (or was) running asynchronously.

The frameDropped bit may be set if the frame was dropped (synchronously).

Pass `NULL` if you do not want to receive this information.

## Discussion

Encoded frames may or may not be output before the function returns. The client should not modify the pixel data after making this call. The session and/or encoder retains the image buffer as long as necessary.

## See Also

### Encoding Frames

func VTCompressionSessionGetPixelBufferPool(VTCompressionSession) -> CVPixelBufferPool?

Returns a pool that provides ideal source pixel buffers for a compression session.

func VTCompressionSessionPrepareToEncodeFrames(VTCompressionSession) -> OSStatus

Enables the encoder to perform any necessary resource allocation before the encoder begins encoding frames (optional).

func VTCompressionSessionEncodeFrame(VTCompressionSession, imageBuffer: CVImageBuffer, presentationTimeStamp: CMTime, duration: CMTime, frameProperties: CFDictionary?, infoFlagsOut: UnsafeMutablePointer&lt;VTEncodeInfoFlags>?, outputHandler: VTCompressionOutputHandler) -> OSStatus

Presents frames to the compression session and invokes the output callback when compression is complete.

func VTCompressionSessionCompleteFrames(VTCompressionSession, untilPresentationTimeStamp: CMTime) -> OSStatus

Forces the compression session to complete the encoding of frames.

