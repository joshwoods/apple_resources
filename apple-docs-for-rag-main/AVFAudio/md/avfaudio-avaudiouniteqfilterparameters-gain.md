

- AVFAudio
- AVAudioUnitEQFilterParameters
-  gain 

Instance Property

# gain

The gain of the equalizer filter, in decibels.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var gain: Float { get set }
```

## Discussion

The default value is `0 dB`. The valid range of values is `-96 dB` through `24 dB`.

## See Also

### Getting and Setting Equalizer Filter Parameters

var bandwidth: Float

The bandwidth of the equalizer filter, in octaves.

var bypass: Bool

The bypass state of the equalizer filter band.

var filterType: AVAudioUnitEQFilterType

The equalizer filter type.

var frequency: Float

The frequency of the equalizer filter, in hertz.

