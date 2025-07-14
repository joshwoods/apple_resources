

- AVFAudio
- AVAudioConverter
-  sampleRateConverterQuality 

Instance Property

# sampleRateConverterQuality

A sample rate converter algorithm key value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var sampleRateConverterQuality: Int { get set }
```

## Discussion

For information about possible key values, see AVSampleRateConverterAlgorithmKey.

## See Also

### Getting Sample Rate Properties

var sampleRateConverterAlgorithm: String?

The priming method the sample rate converter or decoder uses.

var applicableEncodeSampleRates: [NSNumber]?

An array of output sample rates that the converter applies according to the current formats and settings, when encoding.

var availableEncodeSampleRates: [NSNumber]?

An array of all output sample rates the codec provides when encoding.

