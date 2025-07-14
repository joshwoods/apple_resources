

- AVFAudio
- AVAudioConverter
-  bitRate 

Instance Property

# bitRate

The bit rate, in bits per second.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var bitRate: Int { get set }
```

## Discussion

This value only applies when encoding.

## See Also

### Getting Bit Rate Properties

var applicableEncodeBitRates: [NSNumber]?

An array of bit rates the framework applies during encoding according to the current formats and settings.

var availableEncodeBitRates: [NSNumber]?

An array of all bit rates the codec provides when encoding.

var availableEncodeChannelLayoutTags: [NSNumber]?

An array of all output channel layout tags the codec provides when encoding.

var bitRateStrategy: String?

A key value constant the framework uses during encoding.

