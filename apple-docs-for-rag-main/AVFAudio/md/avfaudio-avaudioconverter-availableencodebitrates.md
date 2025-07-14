

- AVFAudio
- AVAudioConverter
-  availableEncodeBitRates 

Instance Property

# availableEncodeBitRates

An array of all bit rates the codec provides when encoding.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var availableEncodeBitRates: [NSNumber]? { get }
```

## Discussion

This property returns `nil` if you’re not encoding.

## See Also

### Getting Bit Rate Properties

var applicableEncodeBitRates: [NSNumber]?

An array of bit rates the framework applies during encoding according to the current formats and settings.

var availableEncodeChannelLayoutTags: [NSNumber]?

An array of all output channel layout tags the codec provides when encoding.

var bitRate: Int

The bit rate, in bits per second.

var bitRateStrategy: String?

A key value constant the framework uses during encoding.

