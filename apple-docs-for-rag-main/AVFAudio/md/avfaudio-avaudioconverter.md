

- AVFAudio
-  AVAudioConverter 

Class

# AVAudioConverter

An object that converts streams of audio between formats.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioConverter
```

## Overview

The audio converter class transforms audio between file formats and audio encodings.

Supported transformations include:

- PCM float, integer, or bit depth conversions

- PCM sample rate conversion

- PCM interleaving and deinterleaving

- Encoding PCM to compressed formats

- Decoding compressed formats to PCM

A single audio converter instance may perform more than one of the above transformations.

## Topics

### Creating an Audio Converter

init?(from: AVAudioFormat, to: AVAudioFormat)

Creates an audio converter object from the specified input and output formats.

### Converting Audio Formats

func convert(to: AVAudioBuffer, error: NSErrorPointer, withInputFrom: AVAudioConverterInputBlock) -> AVAudioConverterOutputStatus

Performs a conversion between audio formats, if the system supports it.

func convert(to: AVAudioPCMBuffer, from: AVAudioPCMBuffer) throws

Performs a basic conversion between audio formats that doesn’t involve converting codecs or sample rates.

enum AVAudioConverterInputStatus

An option that indicates the status of an audio converter input block.

enum AVAudioConverterOutputStatus

An option that indicates the return status of an audio converter method.

### Resetting an Audio Converter

func reset()

Resets the converter so you can convert a new audio stream.

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

var maximumOutputPacketSize: Int

The maximum size of an output packet, in bytes.

### Getting Bit Rate Properties

var applicableEncodeBitRates: [NSNumber]?

An array of bit rates the framework applies during encoding according to the current formats and settings.

var availableEncodeBitRates: [NSNumber]?

An array of all bit rates the codec provides when encoding.

var availableEncodeChannelLayoutTags: [NSNumber]?

An array of all output channel layout tags the codec provides when encoding.

var bitRate: Int

The bit rate, in bits per second.

var bitRateStrategy: String?

A key value constant the framework uses during encoding.

### Getting Sample Rate Properties

var sampleRateConverterQuality: Int

A sample rate converter algorithm key value.

var sampleRateConverterAlgorithm: String?

The priming method the sample rate converter or decoder uses.

var applicableEncodeSampleRates: [NSNumber]?

An array of output sample rates that the converter applies according to the current formats and settings, when encoding.

var availableEncodeSampleRates: [NSNumber]?

An array of all output sample rates the codec provides when encoding.

### Getting Priming Information

var primeInfo: AVAudioConverterPrimeInfo

The number of priming frames the converter uses.

var primeMethod: AVAudioConverterPrimeMethod

The priming method the sample rate converter or decoder uses.

struct AVAudioConverterPrimeInfo

Priming information for audio conversion.

enum AVAudioConverterPrimeMethod

Options for the prime method property.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

