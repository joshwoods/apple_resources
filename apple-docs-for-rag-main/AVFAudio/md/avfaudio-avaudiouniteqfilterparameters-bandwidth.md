

- AVFAudio
- AVAudioUnitEQFilterParameters
-  bandwidth 

Instance Property

# bandwidth

The bandwidth of the equalizer filter, in octaves.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var bandwidth: Float { get set }
```

## Discussion

The value range of values is `0.05` to `5.0` octaves.

## See Also

### Getting and Setting Equalizer Filter Parameters

var bypass: Bool

The bypass state of the equalizer filter band.

var filterType: AVAudioUnitEQFilterType

The equalizer filter type.

var frequency: Float

The frequency of the equalizer filter, in hertz.

var gain: Float

The gain of the equalizer filter, in decibels.

