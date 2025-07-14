

- MediaExtension
-  kMEVideoDecoderObjectNameKey 

Global Variable

# kMEVideoDecoderObjectNameKey

A user-readable string describing the decoder.

Mac Catalyst 18.0+macOS 15.0+

``` source
var kMEVideoDecoderObjectNameKey: String { get }
```

## Discussion

This string is used internally for uniquely identifying video decoders and possibly for debug logging but is typically not visible to users.

## See Also

### Property list keys

var kMEVideoDecoderClassImplementationIDKey: String

The unique identifier for the video decoder.

var kMERAWProcessorExtensionPointName: String

The extension point name for RAW processors.

var kMEVideoDecoderCodecInfoKey: String

An array of one or more dictionaries describing the codecs that the decoder supports.

var kMEVideoDecoderCodecTypeKey: String

A string describing the four-character code of the codec that the decoder supports.

var kMEVideoDecoderCodecNameKey: String

A user-readable string describing the name of the codec format.

