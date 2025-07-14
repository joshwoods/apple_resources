

- MediaExtension
-  kMEVideoDecoderExtensionPointName 

Global Variable

# kMEVideoDecoderExtensionPointName

The extension point name for video decoders.

Mac Catalyst 18.0+macOS 15.0+

``` source
var kMEVideoDecoderExtensionPointName: String { get }
```

## Discussion

The value for this string is `com.apple.mediaextension.videodecoder`.

## See Also

### Property list keys

var kMEVideoDecoderClassImplementationIDKey: String

The unique identifier for the video decoder.

var kMEVideoDecoderObjectNameKey: String

A user-readable string describing the decoder.

var kMEVideoDecoderCodecInfoKey: String

An array of one or more dictionaries describing the codecs that the decoder supports.

var kMEVideoDecoderCodecTypeKey: String

A string describing the four-character code of the codec that the decoder supports.

var kMEVideoDecoderCodecNameKey: String

A user-readable string describing the name of the codec format.

