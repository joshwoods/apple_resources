

- AVFAudio
- AVAudioConverter
-  downmix 

Instance Property

# downmix

A Boolean value that indicates whether the framework mixes the channels instead of remapping.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var downmix: Bool { get set }
```

## Discussion

This property defaults to `false`, indicating that the framework remaps the channels. When `true`, and channel remapping is necessary, the framework mixes the channels.

## See Also

### Getting Audio Converter Properties

var channelMap: [NSNumber]

An array of integers that indicates which input to derive each output from.

var dither: Bool

A Boolean value that indicates whether dither is on.

var inputFormat: AVAudioFormat

The format of the input audio stream.

var outputFormat: AVAudioFormat

The format of the output audio stream.

var magicCookie: Data?

An object that contains metadata for encoders and decoders.

var maximumOutputPacketSize: Int

The maximum size of an output packet, in bytes.

