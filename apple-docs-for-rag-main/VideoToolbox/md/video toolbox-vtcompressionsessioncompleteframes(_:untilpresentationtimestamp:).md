

- Video Toolbox
-  VTCompressionSessionCompleteFrames(\_:untilPresentationTimeStamp:) 

Function

# VTCompressionSessionCompleteFrames(\_:untilPresentationTimeStamp:)

Forces the compression session to complete the encoding of frames.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTCompressionSessionCompleteFrames(
    _ session: VTCompressionSession,
    untilPresentationTimeStamp completeUntilPresentationTimeStamp: CMTime
) -> OSStatus
```

## Parameters 

`session`  

The compression session.

`completeUntilPresentationTimeStamp`  

The timestamp at which to complete frame encoding.

## Discussion

If `completeUntilPresentationTimeStamp` is numeric, frames with presentation timestamps up to and including this timestamp are emitted before the function returns.

If `completeUntilPresentationTimeStamp` is non-numeric, all pending frames are emitted before the function returns.

## See Also

### Encoding Frames

func VTCompressionSessionGetPixelBufferPool(VTCompressionSession) -> CVPixelBufferPool?

Returns a pool that provides ideal source pixel buffers for a compression session.

func VTCompressionSessionPrepareToEncodeFrames(VTCompressionSession) -> OSStatus

Enables the encoder to perform any necessary resource allocation before the encoder begins encoding frames (optional).

func VTCompressionSessionEncodeFrame(VTCompressionSession, imageBuffer: CVImageBuffer, presentationTimeStamp: CMTime, duration: CMTime, frameProperties: CFDictionary?, sourceFrameRefcon: UnsafeMutableRawPointer?, infoFlagsOut: UnsafeMutablePointer&lt;VTEncodeInfoFlags>?) -> OSStatus

Presents frames to the compression session.

func VTCompressionSessionEncodeFrame(VTCompressionSession, imageBuffer: CVImageBuffer, presentationTimeStamp: CMTime, duration: CMTime, frameProperties: CFDictionary?, infoFlagsOut: UnsafeMutablePointer&lt;VTEncodeInfoFlags>?, outputHandler: VTCompressionOutputHandler) -> OSStatus

Presents frames to the compression session and invokes the output callback when compression is complete.

