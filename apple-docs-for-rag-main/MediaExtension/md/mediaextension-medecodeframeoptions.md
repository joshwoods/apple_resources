

- MediaExtension
-  MEDecodeFrameOptions 

Class

# MEDecodeFrameOptions

An object that guides the video decoder operation on a per-frame basis.

macOS 14.0+

``` source
class MEDecodeFrameOptions
```

## Topics

### Inspecting frame decoding options

var doNotOutputFrame: Bool

A Boolean value that hints to the decoder whether or not it should emit an image buffer for the frame.

var realTimePlayback: Bool

A Boolean value that hints to the decoder to use a low-power mode that can’t decode faster than 1x real-time.

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

class MEVideoDecoderPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

Video decoder property list dictionary

Include a property list dictionary to describe a video decoder.

Video decoder entitlement

Include an entitlement to indicate your extension is a MediaExtension video decoder.

