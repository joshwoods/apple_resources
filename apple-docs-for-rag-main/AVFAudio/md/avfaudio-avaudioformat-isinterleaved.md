

- AVFAudio
- AVAudioFormat
-  isInterleaved 

Instance Property

# isInterleaved

A Boolean value that indicates whether the samples mix into one stream.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isInterleaved: Bool { get }
```

## Discussion

This value is only valid for PCM formats.

## See Also

### Determining the Audio Format

var isStandard: Bool

A Boolean value that indicates whether the format is in a deinterleaved native-endian float state.

var commonFormat: AVAudioCommonFormat

The common format identifier instance.

var settings: [String : Any]

A dictionary that represents the format as a dictionary using audio setting keys.

var magicCookie: Data?

An object that contains metadata that encoders and decoders require.

