

- MediaExtension
-  kMEVideoDecoderCodecInfoKey 

Global Variable

# kMEVideoDecoderCodecInfoKey

An array of one or more dictionaries describing the codecs that the decoder supports.

Mac Catalyst 18.0+macOS 15.0+

``` source
var kMEVideoDecoderCodecInfoKey: String { get }
```

## Discussion

Each dictionary must contain the name and the codec format type key.

## See Also

### Property list keys

var kMEVideoDecoderClassImplementationIDKey: String

The unique identifier for the video decoder.

var kMERAWProcessorExtensionPointName: String

The extension point name for RAW processors.

var kMEVideoDecoderObjectNameKey: String

A user-readable string describing the decoder.

var kMEVideoDecoderCodecTypeKey: String

A string describing the four-character code of the codec that the decoder supports.

var kMEVideoDecoderCodecNameKey: String

A user-readable string describing the name of the codec format.

