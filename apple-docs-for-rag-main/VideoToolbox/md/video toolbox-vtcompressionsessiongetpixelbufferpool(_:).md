

- Video Toolbox
-  VTCompressionSessionGetPixelBufferPool(\_:) 

Function

# VTCompressionSessionGetPixelBufferPool(\_:)

Returns a pool that provides ideal source pixel buffers for a compression session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTCompressionSessionGetPixelBufferPool(_ session: VTCompressionSession) -> CVPixelBufferPool?
```

## Parameters 

`session`  

The compression session.

## Return Value

A configured pixel buffer pool.

## Discussion

The compression session creates this pixel buffer pool based on the compressor’s pixel buffer attributes and any pixel buffer attributes passed in to VTCompressionSessionCreate(allocator:width:height:codecType:encoderSpecification:imageBufferAttributes:compressedDataAllocator:outputCallback:refcon:compressionSessionOut:). If the source pixel buffer attributes and the compressor pixel buffer attributes cannot be reconciled, the pool is based on the source pixel buffer attributes, and VideoToolbox converts each CVImageBuffer internally.

Note

Clients can call this function once and retain the resulting pool, but the call is cheap enough that it’s ok to call it once per frame. If a change of session properties causes the compressor’s pixel buffer attributes to change, it’s possible that this function might return a different pool.

## See Also

### Encoding Frames

func VTCompressionSessionPrepareToEncodeFrames(VTCompressionSession) -> OSStatus

Enables the encoder to perform any necessary resource allocation before the encoder begins encoding frames (optional).

func VTCompressionSessionEncodeFrame(VTCompressionSession, imageBuffer: CVImageBuffer, presentationTimeStamp: CMTime, duration: CMTime, frameProperties: CFDictionary?, sourceFrameRefcon: UnsafeMutableRawPointer?, infoFlagsOut: UnsafeMutablePointer&lt;VTEncodeInfoFlags>?) -> OSStatus

Presents frames to the compression session.

func VTCompressionSessionEncodeFrame(VTCompressionSession, imageBuffer: CVImageBuffer, presentationTimeStamp: CMTime, duration: CMTime, frameProperties: CFDictionary?, infoFlagsOut: UnsafeMutablePointer&lt;VTEncodeInfoFlags>?, outputHandler: VTCompressionOutputHandler) -> OSStatus

Presents frames to the compression session and invokes the output callback when compression is complete.

func VTCompressionSessionCompleteFrames(VTCompressionSession, untilPresentationTimeStamp: CMTime) -> OSStatus

Forces the compression session to complete the encoding of frames.

