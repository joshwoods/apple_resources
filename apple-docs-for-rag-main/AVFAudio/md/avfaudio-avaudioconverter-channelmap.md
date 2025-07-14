

- AVFAudio
- AVAudioConverter
-  channelMap 

Instance Property

# channelMap

An array of integers that indicates which input to derive each output from.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var channelMap: [NSNumber] { get set }
```

## Discussion

The array size equals the number of output channels. Each element’s value is the input channel number, starting with zero, that the framework copies to that output.

A negative value means that the output channel doesn’t have a source and is silent.

Setting a channel map overrides channel mapping due to any channel layouts in the input and output formats that you supply.

## See Also

### Getting Audio Converter Properties

var dither: Bool

A Boolean value that indicates whether dither is on.

var downmix: Bool

A Boolean value that indicates whether the framework mixes the channels instead of remapping.

var inputFormat: AVAudioFormat

The format of the input audio stream.

var outputFormat: AVAudioFormat

The format of the output audio stream.

var magicCookie: Data?

An object that contains metadata for encoders and decoders.

var maximumOutputPacketSize: Int

The maximum size of an output packet, in bytes.

