

- AVFAudio
- AVAudioConverter
-  bitRateStrategy 

Instance Property

# bitRateStrategy

A key value constant the framework uses during encoding.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var bitRateStrategy: String? { get set }
```

## Discussion

This property returns `nil` if you’re not encoding. For information about possible values, see AVEncoderBitRateStrategyKey.

## See Also

### Getting Bit Rate Properties

var applicableEncodeBitRates: [NSNumber]?

An array of bit rates the framework applies during encoding according to the current formats and settings.

var availableEncodeBitRates: [NSNumber]?

An array of all bit rates the codec provides when encoding.

var availableEncodeChannelLayoutTags: [NSNumber]?

An array of all output channel layout tags the codec provides when encoding.

var bitRate: Int

The bit rate, in bits per second.

