

- Video Toolbox
-  VTDecompressionMultiImageCapableOutputHandler 

Type Alias

# VTDecompressionMultiImageCapableOutputHandler

A type alias for callback that the system invokes when it finishes decompressing a frame.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
typealias VTDecompressionMultiImageCapableOutputHandler = (OSStatus, VTDecodeInfoFlags, CVImageBuffer?, __CMTaggedBufferGroup?, CMTime, CMTime) -> Void
```

## Parameters 

`status`  

A value of `noErr` if decompression succeeds; otherwise, an error code if decompression fails.

`infoFlags`  

A VTEncodeInfoFlags pointer to receive information about the decode operation.

The asynchronous bit may be set if the decode is (or was) running asynchronously.

The frameDropped bit may be set if the frame was dropped (synchronously).

Pass `NULL` if you don’t want to receive this information.

`imageBuffer`  

The decompressed pixel buffer.

`taggedBufferGroup`  

A CMTaggedBufferGroupRef that contains the multiple images for the decompressed frame, if the decompression succeeds; otherwise, `NULL`.

`presentationTimeStamp`  

The frame’s presentation timestamp; otherwise, invalid if the value isn’t available.

`presentationDuration`  

The frame’s presentation duration; otherwise, invalid if the value isn’t available.

## Discussion

Pass a callback of this type to VTDecompressionSessionDecodeFrameWithMultiImageCapableOutputHandler to handle the decompressed frame output. The system doesn’t necessarily invoke the callback in display order. If the multi-image decompression call returns an error, the system doesn’t call this block.

Important

The video decompressor may still reference the pixel buffers that this callback provides if the imageBufferModifiable flag isn’t set. It’s not safe to modify the returned pixel buffers in this state.

## See Also

### Decoding Multi-Image Frames

func VTIsStereoMVHEVCDecodeSupported() -> Bool

Returns a Boolean value that indicates whether the system supports MV-HEVC decoding.

