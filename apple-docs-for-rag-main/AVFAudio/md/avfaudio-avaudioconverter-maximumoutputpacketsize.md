

- AVFAudio
- AVAudioConverter
-  maximumOutputPacketSize 

Instance Property

# maximumOutputPacketSize

The maximum size of an output packet, in bytes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var maximumOutputPacketSize: Int { get }
```

## See Also

### Getting Audio Converter Properties

var channelMap: [NSNumber]

An array of integers that indicates which input to derive each output from.

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

