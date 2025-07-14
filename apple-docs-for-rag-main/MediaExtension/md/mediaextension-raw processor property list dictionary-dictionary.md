

- MediaExtension
-  RAW processor property list dictionary 

API Collection

# RAW processor property list dictionary

Include a property list dictionary to describe a RAW processor.

## Overview

A MediaExtension RAW processor needs to include an `EXAppExtensionAttributes` dictionary in its `Info.plist` file that contains the following keys and values:

- kMEVideoDecoderClassImplementationIDKey: The identifier for the RAW processor. Format similarly to the bundle identifier. The key is the same as for video decoders.

- `EXExtensionPointIdentifier`: The extension point name for RAW processors. Set to the value for kMERAWProcessorExtensionPointName.

- `EXPrincipalClass`: The name of the RAW processor factory class that conforms to the MERAWProcessorExtension protocol.

- kMEVideoDecoderObjectNameKey: A user-readable string that describes RAW processor. This string is used for uniquely identifying RAW processors and possibly for debug logging but is typically not visible to users. The key is the same as for video decoders.

- kMEVideoDecoderCodecInfoKey: An array of one or more dictionaries describing the formats that the RAW processor supports. The key is the same as for video decoders. Each dictionary must include the following keys:

  - kMEVideoDecoderCodecTypeKey: A string describing the four-character code of the codec associated with the video decoder. Each string should be exactly four characters long and use ASCII character set encoding. The key is the same as for video decoders.

  - kMEVideoDecoderCodecNameKey: A user-readable string describing the name of the codec format. This string might be displayed as format information for the video track in a player application. The key is the same as for video decoders.

## Topics

### Property list keys

var kMEVideoDecoderClassImplementationIDKey: String

The unique identifier for the video decoder.

var kMERAWProcessorExtensionPointName: String

The extension point name for RAW processors.

var kMEVideoDecoderObjectNameKey: String

A user-readable string describing the decoder.

var kMEVideoDecoderCodecInfoKey: String

An array of one or more dictionaries describing the codecs that the decoder supports.

var kMEVideoDecoderCodecTypeKey: String

A string describing the four-character code of the codec that the decoder supports.

var kMEVideoDecoderCodecNameKey: String

A user-readable string describing the name of the codec format.

## See Also

### RAW processors

protocol MERAWProcessor

A protocol that defines the requirements for a RAW processor.

protocol MERAWProcessorExtension

A protocol that defines a factory to create RAW processors for a codec type that the extension implements.

class MERAWProcessorPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

class MERAWProcessingParameter

An object for the RAW processor to describe each processing parameter the processor exposes.

enum MERAWProcessorNotification

Notifications that indicate a RAW processor state change.

RAW processor entitlement

Include an entitlement to indicate your extension is a MediaExtension RAW processor.

