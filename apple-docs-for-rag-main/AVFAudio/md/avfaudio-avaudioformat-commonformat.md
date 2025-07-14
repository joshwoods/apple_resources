

- AVFAudio
- AVAudioFormat
-  commonFormat 

Instance Property

# commonFormat

The common format identifier instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var commonFormat: AVAudioCommonFormat { get }
```

## See Also

### Determining the Audio Format

var isInterleaved: Bool

A Boolean value that indicates whether the samples mix into one stream.

var isStandard: Bool

A Boolean value that indicates whether the format is in a deinterleaved native-endian float state.

var settings: [String : Any]

A dictionary that represents the format as a dictionary using audio setting keys.

var magicCookie: Data?

An object that contains metadata that encoders and decoders require.

