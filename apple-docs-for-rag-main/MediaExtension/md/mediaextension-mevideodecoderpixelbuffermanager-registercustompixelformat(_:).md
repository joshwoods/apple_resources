

- MediaExtension
- MEVideoDecoderPixelBufferManager
-  registerCustomPixelFormat(\_:) 

Instance Method

# registerCustomPixelFormat(\_:)

macOS 14.0+

``` source
func registerCustomPixelFormat(_ customPixelFormat: [String : Any])
```

## Parameters 

`customPixelFormat`  

A dictionary containing a set of keys and values as described in CVPixelFormatDescription suitable for providing as the ‘description’ parameter to CVPixelFormatDescriptionCreateWithPixelFormatType(_:_:). This must contain the custom pixel format fourCC as the value for the `kCVPixelFormatCodecType` key.

## Discussion

This property is appropriate for decoders which produce output in a custom pixel format. This will generally only be used by decoders which produce RAW output, where the decoder’s output buffers will only be consumed by an MERAWProcessor extension which registers the same pixel format. The MERAWProcessor needs to manually register the custom pixel format using CVPixelFormatDescriptionCreateWithPixelFormatType(_:_:).

