

- Video Toolbox
-  VTDecompressionSessionCanAcceptFormatDescription(\_:formatDescription:) 

Function

# VTDecompressionSessionCanAcceptFormatDescription(\_:formatDescription:)

Indicates whether the session can decode frames with the given format description.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTDecompressionSessionCanAcceptFormatDescription(
    _ session: VTDecompressionSession,
    formatDescription newFormatDesc: CMFormatDescription
) -> Bool
```

## Parameters 

`session`  

The decompression session.

`newFormatDesc`  

The CMFormatDescription to test.

## Return Value

true if the decompression session accepts the format description; otherwise, false.

## Discussion

Some video decoders can accommodate minor changes in format without needing to be completely reset in a new session. Use this function to test whether a format change is sufficiently minor.

## See Also

### Decoding Frames

func VTDecompressionSessionDecodeFrame(VTDecompressionSession, sampleBuffer: CMSampleBuffer, flags: VTDecodeFrameFlags, frameRefcon: UnsafeMutableRawPointer?, infoFlagsOut: UnsafeMutablePointer&lt;VTDecodeInfoFlags>?) -> OSStatus

Decompresses a video frame.

func VTDecompressionSessionDecodeFrame(VTDecompressionSession, sampleBuffer: CMSampleBuffer, flags: VTDecodeFrameFlags, infoFlagsOut: UnsafeMutablePointer&lt;VTDecodeInfoFlags>?, outputHandler: VTDecompressionOutputHandler) -> OSStatus

Decompresses a video frame and invokes the output callback when the decompression completes.

func VTDecompressionSessionDecodeFrame(VTDecompressionSession, sampleBuffer: CMSampleBuffer, flags: VTDecodeFrameFlags, infoFlagsOut: UnsafeMutablePointer&lt;VTDecodeInfoFlags>?, completionHandler: (OSStatus, VTDecodeInfoFlags, CVImageBuffer?, [CMTaggedBuffer]?, CMTime, CMTime) -> Void) -> OSStatus

Decompresses a video frame and calls the provided output closure when decompression completes.

func VTDecompressionSessionFinishDelayedFrames(VTDecompressionSession) -> OSStatus

Directs the decompression session to emit all delayed frames.

func VTDecompressionSessionWaitForAsynchronousFrames(VTDecompressionSession) -> OSStatus

Waits for any and all outstanding asynchronous and delayed frames to complete, then returns.

func VTDecompressionSessionCopyBlackPixelBuffer(VTDecompressionSession, pixelBufferOut: UnsafeMutablePointer&lt;CVPixelBuffer?>) -> OSStatus

Copies a black pixel buffer from the decompression session.

