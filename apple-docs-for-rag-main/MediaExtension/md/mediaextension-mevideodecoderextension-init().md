

- MediaExtension
- MEVideoDecoderExtension
-  init() 

Initializer

# init()

Creates a new video decoder factory.

macOS 14.0+

``` source
init()
```

**Required**

## See Also

### Creating a video decoder

func makeVideoDecoder(codecType: CMVideoCodecType, videoFormatDescription: CMVideoFormatDescription, videoDecoderSpecifications: [String : Any], pixelBufferManager: MEVideoDecoderPixelBufferManager) throws -> any MEVideoDecoder

Creates a new video decoder that matches the codec type, format description, decoder specifications, and pixel buffer manager that you specify.

**Required**

