

- AVFAudio
- AVAudioConverter
-  applicableEncodeSampleRates 

Instance Property

# applicableEncodeSampleRates

An array of output sample rates that the converter applies according to the current formats and settings, when encoding.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var applicableEncodeSampleRates: [NSNumber]? { get }
```

## Discussion

This property returns `nil` if you’re not encoding.

## See Also

### Getting Sample Rate Properties

var sampleRateConverterQuality: Int

A sample rate converter algorithm key value.

var sampleRateConverterAlgorithm: String?

The priming method the sample rate converter or decoder uses.

var availableEncodeSampleRates: [NSNumber]?

An array of all output sample rates the codec provides when encoding.

