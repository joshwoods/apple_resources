

- Video Toolbox
-  VTDecompressionSessionDecodeFrame(\_:sampleBuffer:flags:frameRefcon:infoFlagsOut:) 

Function

# VTDecompressionSessionDecodeFrame(\_:sampleBuffer:flags:frameRefcon:infoFlagsOut:)

Decompresses a video frame.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTDecompressionSessionDecodeFrame(
    _ session: VTDecompressionSession,
    sampleBuffer: CMSampleBuffer,
    flags decodeFlags: VTDecodeFrameFlags,
    frameRefcon sourceFrameRefCon: UnsafeMutableRawPointer?,
    infoFlagsOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`session`  

The decompression session.

`sampleBuffer`  

A CMSampleBuffer object containing one or more video frames.

`decodeFlags`  

A bitfield of directives to the decompression session and decoder.

The kVTDecodeFrame_EnableAsynchronousDecompression bit indicates whether the video decoder may decompress the frame asynchronously.

The kVTDecodeFrame_EnableTemporalProcessing bit indicates whether the decoder may delay calls to the output callback so as to enable processing in temporal (display) order.

If both flags are clear, the decompression completes and your output callback function will be called before `VTDecompressionSessionDecodeFrame` returns. If either flag is set, `VTDecompressionSessionDecodeFrame` may return before the output callback function is called.

`sourceFrameRefCon`  

Your reference value for the frame. Note that if `sampleBuffer` contains multiple frames, the output callback function is called multiple times with this `sourceFrameRefCon` value.

`infoFlagsOut`  

A VTEncodeInfoFlags pointer to receive information about the decode operation.

The asynchronous bit may be set if the decode is (or was) running asynchronously.

The frameDropped bit may be set if the frame was dropped (synchronously).

Pass `NULL` if you do not want to receive this information.

## Return Value

An `OSStatus` value that indicates the result of the operation.

## See Also

### Decoding Frames

func VTDecompressionSessionCanAcceptFormatDescription(VTDecompressionSession, formatDescription: CMFormatDescription) -> Bool

Indicates whether the session can decode frames with the given format description.

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

