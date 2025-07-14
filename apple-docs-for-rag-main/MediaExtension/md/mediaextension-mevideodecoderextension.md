

- MediaExtension
-  MEVideoDecoderExtension 

Protocol

# MEVideoDecoderExtension

A protocol that defines a factory to create new video decoders for a codec type that the extension implements.

macOS 14.0+

``` source
protocol MEVideoDecoderExtension : NSObjectProtocol
```

## Discussion

This protocol provides a factory method to create a new MEVideoDecoder instance for a codecType implemented by the extension. A single MEVideoDecoderExtension is instantiated by the `VideoToolbox`, and will be called to create individual MEVideoDecoder instances as needed. If the codecType or `FormatDescription` passed to makeVideoDecoder(codecType:videoFormatDescription:videoDecoderSpecifications:pixelBufferManager:) is not compatible with the MEVideoDecoder implementation, the factory call should fail and return MEError.Code.unsupportedFeature.

## Topics

### Creating a video decoder

init()

Creates a new video decoder factory.

**Required**

func makeVideoDecoder(codecType: CMVideoCodecType, videoFormatDescription: CMVideoFormatDescription, videoDecoderSpecifications: [String : Any], pixelBufferManager: MEVideoDecoderPixelBufferManager) throws -> any MEVideoDecoder

Creates a new video decoder that matches the codec type, format description, decoder specifications, and pixel buffer manager that you specify.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Video decoders

protocol MEVideoDecoder

A protocol that defines the requirements for a video decoder.

class MEDecodeFrameOptions

An object that guides the video decoder operation on a per-frame basis.

class MEVideoDecoderPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

Video decoder property list dictionary

Include a property list dictionary to describe a video decoder.

Video decoder entitlement

Include an entitlement to indicate your extension is a MediaExtension video decoder.

