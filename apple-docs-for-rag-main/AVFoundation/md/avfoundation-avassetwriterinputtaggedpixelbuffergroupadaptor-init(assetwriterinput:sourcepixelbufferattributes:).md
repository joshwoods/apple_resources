

- AVFoundation
- AVAssetWriterInputTaggedPixelBufferGroupAdaptor
-  init(assetWriterInput:sourcePixelBufferAttributes:) 

Initializer

# init(assetWriterInput:sourcePixelBufferAttributes:)

Creates an object that appends tagged buffer groups to an asset writer input.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
init(
    assetWriterInput input: AVAssetWriterInput,
    sourcePixelBufferAttributes: [String : Any]? = nil
)
```

## Parameters 

`input`  

An asset writer input, that handles media data of type video, to use for appending tagged buffer groups.

It’s an error to initialize an adaptor with an asset writer input that is already attached to another instance of tagged pixel buffer group adaptor, or to one th that progresses beyond its AVAssetWriter.Status.unknown state.

`sourcePixelBufferAttributes`  

Specifies the attributes of pixel buffers that the adaptor’s pixel buffer pool vends. If your app doesn’t require a pixel buffer pool, this this value to `nil`.

## Discussion

To take advantage of the improved efficiency of appending buffers created from the adaptor’s pixel buffer pool, specify pixel buffer attributes that most closely accommodate the source format of the video frames of tagged buffer groups to append.

Pixel buffer attributes keys for the pixel buffer pool are defined in ``. To specify the pixel format type, the pixel buffer attributes dictionary should contain a value for kCVPixelBufferPixelFormatTypeKey. For example, specify a format of kCVPixelFormatType_32BGRA for 8-bit-per-channel BGRA. See append(_:withPresentationTime:) in AVAssetWriterInputPixelBufferAdaptor for more information on choosing a pixel format.

