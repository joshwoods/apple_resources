

- MediaExtension
-  MEVideoDecoderPixelBufferManager 

Class

# MEVideoDecoderPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

macOS 14.0+

``` source
class MEVideoDecoderPixelBufferManager
```

## Discussion

Contains the interfaces that the MEVideoDecoder uses for two tasks. First, to declare its set of requirements for output `CVPixelBuffer` objects in the form of a pixelBufferAttributes dictionary. Second, to create pixel buffers that match decoder output requirements but also satisfy Video Toolbox and client requirements.

## Topics

### Creating a pixel buffer

var pixelBufferAttributes: [String : Any]

A dictionary that contains the attributes Video Toolbox uses to create a pixel buffer for the decoder.

func makePixelBuffer() throws -> CVPixelBuffer

Generates a pixel buffer using the session’s pixel buffer pool.

### Registering Custom Pixel Formats

func registerCustomPixelFormat([String : Any])

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Video decoders

protocol MEVideoDecoder

A protocol that defines the requirements for a video decoder.

protocol MEVideoDecoderExtension

A protocol that defines a factory to create new video decoders for a codec type that the extension implements.

class MEDecodeFrameOptions

An object that guides the video decoder operation on a per-frame basis.

Video decoder property list dictionary

Include a property list dictionary to describe a video decoder.

Video decoder entitlement

Include an entitlement to indicate your extension is a MediaExtension video decoder.

