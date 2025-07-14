

- MediaExtension
-  Video decoder property list dictionary 

API Collection

# Video decoder property list dictionary

Include a property list dictionary to describe a video decoder.

## Overview

A MediaExtension video decoder needs to include an `EXAppExtensionAttributes` dictionary in its `Info.plist` file that contains the following keys and values:

- kMEVideoDecoderClassImplementationIDKey: The identifier for the decoder. Format similarly to the bundle identifier.

- `EXExtensionPointIdentifier`: The extension point name for video decoders. Set to the value for kMEVideoDecoderExtensionPointName.

- `EXPrincipalClass`: The name of the video decoder factory class that conforms to the MEVideoDecoderExtension protocol.

- kMEVideoDecoderObjectNameKey: A user-readable string that describes the codec format. This string is used for uniquely identifying video decoders and possibly for debug logging but is typically not visible to users.

- kMEVideoDecoderCodecInfoKey: An array of one or more dictionaries describing the formats that the video decoder supports. Each dictionary must include the following keys:

  - kMEVideoDecoderCodecTypeKey: A string describing the four-character code of the codec associated with the video decoder. Each string should be exactly four characters long and use ASCII character set encoding.

  - kMEVideoDecoderCodecNameKey: A user-readable string describing the name of the codec format. This string might be displayed as format information for the video track in a player application.

## Topics

### Property list keys

var kMEVideoDecoderClassImplementationIDKey: String

The unique identifier for the video decoder.

var kMEVideoDecoderExtensionPointName: String

The extension point name for video decoders.

var kMEVideoDecoderObjectNameKey: String

A user-readable string describing the decoder.

var kMEVideoDecoderCodecInfoKey: String

An array of one or more dictionaries describing the codecs that the decoder supports.

var kMEVideoDecoderCodecTypeKey: String

A string describing the four-character code of the codec that the decoder supports.

var kMEVideoDecoderCodecNameKey: String

A user-readable string describing the name of the codec format.

## See Also

### Video decoders

protocol MEVideoDecoder

A protocol that defines the requirements for a video decoder.

protocol MEVideoDecoderExtension

A protocol that defines a factory to create new video decoders for a codec type that the extension implements.

class MEDecodeFrameOptions

An object that guides the video decoder operation on a per-frame basis.

class MEVideoDecoderPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

Video decoder entitlement

Include an entitlement to indicate your extension is a MediaExtension video decoder.

