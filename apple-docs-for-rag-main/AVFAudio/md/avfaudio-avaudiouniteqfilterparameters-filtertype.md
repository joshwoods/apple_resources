

- AVFAudio
- AVAudioUnitEQFilterParameters
-  filterType 

Instance Property

# filterType

The equalizer filter type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var filterType: AVAudioUnitEQFilterType { get set }
```

## Discussion

The default value is AVAudioUnitEQFilterType.parametric.

## See Also

### Getting and Setting Equalizer Filter Parameters

var bandwidth: Float

The bandwidth of the equalizer filter, in octaves.

var bypass: Bool

The bypass state of the equalizer filter band.

var frequency: Float

The frequency of the equalizer filter, in hertz.

var gain: Float

The gain of the equalizer filter, in decibels.

