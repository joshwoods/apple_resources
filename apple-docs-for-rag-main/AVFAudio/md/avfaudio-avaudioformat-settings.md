

- AVFAudio
- AVAudioFormat
-  settings 

Instance Property

# settings

A dictionary that represents the format as a dictionary using audio setting keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var settings: [String : Any] { get }
```

## Discussion

The settings dictionary doesn’t support all formats that AudioStreamBasicDescription represents (the underlying implementation), in which case, this property returns `nil`.

## See Also

### Determining the Audio Format

var isInterleaved: Bool

A Boolean value that indicates whether the samples mix into one stream.

var isStandard: Bool

A Boolean value that indicates whether the format is in a deinterleaved native-endian float state.

var commonFormat: AVAudioCommonFormat

The common format identifier instance.

var magicCookie: Data?

An object that contains metadata that encoders and decoders require.

