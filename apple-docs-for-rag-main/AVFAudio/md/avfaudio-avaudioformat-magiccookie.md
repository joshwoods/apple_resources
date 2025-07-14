

- AVFAudio
- AVAudioFormat
-  magicCookie 

Instance Property

# magicCookie

An object that contains metadata that encoders and decoders require.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var magicCookie: Data? { get set }
```

## Discussion

Encoders produce a `magicCookie` object, and some decoders require it to decode properly.

## See Also

### Determining the Audio Format

var isInterleaved: Bool

A Boolean value that indicates whether the samples mix into one stream.

var isStandard: Bool

A Boolean value that indicates whether the format is in a deinterleaved native-endian float state.

var commonFormat: AVAudioCommonFormat

The common format identifier instance.

var settings: [String : Any]

A dictionary that represents the format as a dictionary using audio setting keys.

