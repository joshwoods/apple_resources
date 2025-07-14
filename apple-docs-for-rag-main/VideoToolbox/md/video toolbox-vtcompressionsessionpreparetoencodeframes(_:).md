

- Video Toolbox
-  VTCompressionSessionPrepareToEncodeFrames(\_:) 

Function

# VTCompressionSessionPrepareToEncodeFrames(\_:)

Enables the encoder to perform any necessary resource allocation before the encoder begins encoding frames (optional).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 10.2+visionOS 1.0+

``` source
func VTCompressionSessionPrepareToEncodeFrames(_ session: VTCompressionSession) -> OSStatus
```

## Parameters 

`session`  

The compression session.

## Discussion

If this function isn’t called, any necessary resources are allocated on the first VTCompressionSessionEncodeFrame(_:imageBuffer:presentationTimeStamp:duration:frameProperties:sourceFrameRefcon:infoFlagsOut:) call.

Subsequent calls to this function have no effect.

## See Also

### Encoding Frames

func VTCompressionSessionGetPixelBufferPool(VTCompressionSession) -> CVPixelBufferPool?

Returns a pool that provides ideal source pixel buffers for a compression session.

func VTCompressionSessionEncodeFrame(VTCompressionSession, imageBuffer: CVImageBuffer, presentationTimeStamp: CMTime, duration: CMTime, frameProperties: CFDictionary?, sourceFrameRefcon: UnsafeMutableRawPointer?, infoFlagsOut: UnsafeMutablePointer&lt;VTEncodeInfoFlags>?) -> OSStatus

Presents frames to the compression session.

func VTCompressionSessionEncodeFrame(VTCompressionSession, imageBuffer: CVImageBuffer, presentationTimeStamp: CMTime, duration: CMTime, frameProperties: CFDictionary?, infoFlagsOut: UnsafeMutablePointer&lt;VTEncodeInfoFlags>?, outputHandler: VTCompressionOutputHandler) -> OSStatus

Presents frames to the compression session and invokes the output callback when compression is complete.

func VTCompressionSessionCompleteFrames(VTCompressionSession, untilPresentationTimeStamp: CMTime) -> OSStatus

Forces the compression session to complete the encoding of frames.

