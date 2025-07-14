

- Video Toolbox
-  VTDecompressionSessionFinishDelayedFrames(\_:) 

Function

# VTDecompressionSessionFinishDelayedFrames(\_:)

Directs the decompression session to emit all delayed frames.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTDecompressionSessionFinishDelayedFrames(_ session: VTDecompressionSession) -> OSStatus
```

## Parameters 

`session`  

The decompression session.

## Return Value

An `OSStatus` value that indicates the result of the operation.

## Discussion

By default, the decompression session may not delay frames indefinitely; frames may only be indefinitely delayed if the client opts in via kVTDecodeFrame_EnableTemporalProcessing.

Important

This function may return before all delayed frames are emitted. To wait for them, call VTDecompressionSessionWaitForAsynchronousFrames(_:) instead.

## See Also

### Decoding Frames

func VTDecompressionSessionCanAcceptFormatDescription(VTDecompressionSession, formatDescription: CMFormatDescription) -> Bool

Indicates whether the session can decode frames with the given format description.

func VTDecompressionSessionDecodeFrame(VTDecompressionSession, sampleBuffer: CMSampleBuffer, flags: VTDecodeFrameFlags, frameRefcon: UnsafeMutableRawPointer?, infoFlagsOut: UnsafeMutablePointer&lt;VTDecodeInfoFlags>?) -> OSStatus

Decompresses a video frame.

func VTDecompressionSessionDecodeFrame(VTDecompressionSession, sampleBuffer: CMSampleBuffer, flags: VTDecodeFrameFlags, infoFlagsOut: UnsafeMutablePointer&lt;VTDecodeInfoFlags>?, outputHandler: VTDecompressionOutputHandler) -> OSStatus

Decompresses a video frame and invokes the output callback when the decompression completes.

func VTDecompressionSessionDecodeFrame(VTDecompressionSession, sampleBuffer: CMSampleBuffer, flags: VTDecodeFrameFlags, infoFlagsOut: UnsafeMutablePointer&lt;VTDecodeInfoFlags>?, completionHandler: (OSStatus, VTDecodeInfoFlags, CVImageBuffer?, [CMTaggedBuffer]?, CMTime, CMTime) -> Void) -> OSStatus

Decompresses a video frame and calls the provided output closure when decompression completes.

func VTDecompressionSessionWaitForAsynchronousFrames(VTDecompressionSession) -> OSStatus

Waits for any and all outstanding asynchronous and delayed frames to complete, then returns.

func VTDecompressionSessionCopyBlackPixelBuffer(VTDecompressionSession, pixelBufferOut: UnsafeMutablePointer&lt;CVPixelBuffer?>) -> OSStatus

Copies a black pixel buffer from the decompression session.

