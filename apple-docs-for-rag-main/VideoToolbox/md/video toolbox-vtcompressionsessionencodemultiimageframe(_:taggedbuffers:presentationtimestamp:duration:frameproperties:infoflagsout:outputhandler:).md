

- Video Toolbox
-  VTCompressionSessionEncodeMultiImageFrame(\_:taggedBuffers:presentationTimeStamp:duration:frameProperties:infoFlagsOut:outputHandler:) 

Function

# VTCompressionSessionEncodeMultiImageFrame(\_:taggedBuffers:presentationTimeStamp:duration:frameProperties:infoFlagsOut:outputHandler:)

Passes a multi-image frame to a compression session for encoding and provides a callback to handle the output.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func VTCompressionSessionEncodeMultiImageFrame(
    _ session: VTCompressionSession,
    taggedBuffers: [CMTaggedBuffer],
    presentationTimeStamp: CMTime,
    duration: CMTime,
    frameProperties: CFDictionary?,
    infoFlagsOut: UnsafeMutablePointer?,
    outputHandler: @escaping VTCompressionOutputHandler
) -> OSStatus
```

## Parameters 

`session`  

The compression session.

`taggedBuffers`  

An array of CMTaggedBuffer structures that contains the multiple images for a video frame to compress.

`presentationTimeStamp`  

The presentation timestamp for this frame to attach to the sample buffer. Each presentation timestamp that you pass to a session must be greater than the previous one.

`duration`  

The presentation duration for this frame to attach to the sample buffer. Pass a value of invalid if you don’t have duration information.

`frameProperties`  

A dictionary that specifies additional properties for encoding this frame. Some session properties may also change between frames, which affect subsequently encoded frames.

`infoFlagsOut`  

Points to a VTEncodeInfoFlags value to receive information about the encode operation.

The system sets the asynchronous flag if the encode runs asynchronously.

The system sets the frameDropped flag if the encoding process dropped a frame (synchronously).

Pass `NULL` if you don’t want to receive this information.

`outputHandler`  

A callback the system invokes when it completes encoding a frame.

The system may invoke this callback asynchronously, on a different thread from the one that calls VTCompressionSessionEncodeMultiImageFrame(_:taggedBuffers:presentationTimeStamp:duration:frameProperties:infoFlagsOut:outputHandler:).

## Return Value

An `OSStatus` value that indicates the result of the operation.

## Discussion

The system doesn’t guarantee that encoded frames be output before the function returns. The session and encoder retain the image buffer as long as necessary.

You can’t call this function on a session created with a VTCompressionOutputCallback.

Important

Don’t modify the pixel data after making this call.

## See Also

### Encoding Multi-Image Frames

func VTIsStereoMVHEVCEncodeSupported() -> Bool

Returns a Boolean value that indicates whether the system supports MV-HEVC encoding.

