

- MediaExtension
- MEVideoDecoderExtension
-  makeVideoDecoder(codecType:videoFormatDescription:videoDecoderSpecifications:pixelBufferManager:) 

Instance Method

# makeVideoDecoder(codecType:videoFormatDescription:videoDecoderSpecifications:pixelBufferManager:)

Creates a new video decoder that matches the codec type, format description, decoder specifications, and pixel buffer manager that you specify.

macOS 14.0+

``` source
func makeVideoDecoder(
    codecType: CMVideoCodecType,
    videoFormatDescription: CMVideoFormatDescription,
    videoDecoderSpecifications: [String : Any],
    pixelBufferManager extensionDecoderPixelBufferManager: MEVideoDecoderPixelBufferManager
) throws -> any MEVideoDecoder
```

**Required**

## Parameters 

`codecType`  

The codec type for the requested decoder.

`videoFormatDescription`  

An object that describes the video data.

`videoDecoderSpecifications`  

A dictionary that contains video decoder specification values, which may be empty. See Decompression Properties for a list of keys to use.

`extensionDecoderPixelBufferManager`  

A pixel buffer manager.

## Return Value

A new MEVideoDecoder.

## Discussion

The `videoDecoderSpecifications` parameter accepts the following keys:

- kVTVideoDecoderSpecification_EnableHardwareAcceleratedVideoDecoder

- kVTVideoDecoderSpecification_RequireHardwareAcceleratedVideoDecoder

- kVTVideoDecoderSpecification_RequiredDecoderGPURegistryID

- kVTVideoDecoderSpecification_PreferredDecoderGPURegistryID

If the parameter values aren’t compatible with the video decoder, this method fails with the error MEError.Code.unsupportedFeature.

The video decoder needs to retain the pixel buffer manager and use it to allocate and configure output pixel buffers.

## See Also

### Creating a video decoder

init()

Creates a new video decoder factory.

**Required**

