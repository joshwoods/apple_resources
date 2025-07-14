

- AVFAudio
- AVAudioConverter
-  applicableEncodeBitRates 

Instance Property

# applicableEncodeBitRates

An array of bit rates the framework applies during encoding according to the current formats and settings.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var applicableEncodeBitRates: [NSNumber]? { get }
```

## Discussion

This property returns `nil` if you’re not encoding.

## See Also

### Getting Bit Rate Properties

var availableEncodeBitRates: [NSNumber]?

An array of all bit rates the codec provides when encoding.

var availableEncodeChannelLayoutTags: [NSNumber]?

An array of all output channel layout tags the codec provides when encoding.

var bitRate: Int

The bit rate, in bits per second.

var bitRateStrategy: String?

A key value constant the framework uses during encoding.

