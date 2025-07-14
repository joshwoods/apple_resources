

- AVFAudio
- AVAudioConverter
-  sampleRateConverterAlgorithm 

Instance Property

# sampleRateConverterAlgorithm

The priming method the sample rate converter or decoder uses.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var sampleRateConverterAlgorithm: String? { get set }
```

## Topics

### Algorithms

let AVSampleRateConverterAlgorithm_Normal: String

The usual encoder bit rate strategy.

let AVSampleRateConverterAlgorithm_MinimumPhase: String

The minimum phase encoder bit rate strategy.

let AVSampleRateConverterAlgorithm_Mastering: String

The mastering encoder bit rate strategy.

## See Also

### Getting Sample Rate Properties

var sampleRateConverterQuality: Int

A sample rate converter algorithm key value.

var applicableEncodeSampleRates: [NSNumber]?

An array of output sample rates that the converter applies according to the current formats and settings, when encoding.

var availableEncodeSampleRates: [NSNumber]?

An array of all output sample rates the codec provides when encoding.

