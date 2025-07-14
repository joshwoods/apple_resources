

- Video Toolbox
-  VTCompressionSessionCreate(allocator:width:height:codecType:encoderSpecification:imageBufferAttributes:compressedDataAllocator:outputCallback:refcon:compressionSessionOut:) 

Function

# VTCompressionSessionCreate(allocator:width:height:codecType:encoderSpecification:imageBufferAttributes:compressedDataAllocator:outputCallback:refcon:compressionSessionOut:)

Creates an object that compresses video frames.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTCompressionSessionCreate(
    allocator: CFAllocator?,
    width: Int32,
    height: Int32,
    codecType: CMVideoCodecType,
    encoderSpecification: CFDictionary?,
    imageBufferAttributes sourceImageBufferAttributes: CFDictionary?,
    compressedDataAllocator: CFAllocator?,
    outputCallback: VTCompressionOutputCallback?,
    refcon outputCallbackRefCon: UnsafeMutableRawPointer?,
    compressionSessionOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

An allocator for the session. Pass `NULL` to use the default allocator.

`width`  

The pixel width of video frames.

`height`  

The pixel height of video frames.

`codecType`  

The codec type.

`encoderSpecification`  

A video encoder to use. Pass `NULL` to let VideoToolbox choose an encoder.

`sourceImageBufferAttributes`  

Required attributes for source pixel buffers, used when creating a pixel buffer pool for source frames. If you don’t want VideoToolbox to create one for you, pass `NULL`.

Using pixel buffers not allocated by VideoToolbox increases the chance that you’ll have to copy image data.

`compressedDataAllocator`  

An allocator for the compressed data. Pass `NULL` to use the default allocator.

In MacOS 10.12 and later, using a `compressedDataAllocator` may trigger an extra buffer copy.

`outputCallback`  

The callback to invoke with compressed frames. The system may call this function asynchronously, on a different thread from the one that calls VTCompressionSessionEncodeFrame(_:imageBuffer:presentationTimeStamp:duration:frameProperties:sourceFrameRefcon:infoFlagsOut:).

Pass `NULL` only if you’ll be calling VTCompressionSessionEncodeFrame(_:imageBuffer:presentationTimeStamp:duration:frameProperties:infoFlagsOut:outputHandler:) for encoding frames.

`outputCallbackRefCon`  

Client-defined reference value for the output callback.

`compressionSessionOut`  

A pointer to a variable to receive the new compression session.

## Discussion

The session outputs compressed frames through the output callback.

## Topics

### Callbacks

typealias VTCompressionOutputCallback

A callback for the system to invoke when it’s finished compressing a frame.

typealias VTCompressionOutputHandler

A callback for the system to invoke when it’s finished compressing a frame.

