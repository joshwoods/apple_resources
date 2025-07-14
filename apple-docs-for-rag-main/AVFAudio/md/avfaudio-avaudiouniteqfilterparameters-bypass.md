

- AVFAudio
- AVAudioUnitEQFilterParameters
-  bypass 

Instance Property

# bypass

The bypass state of the equalizer filter band.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var bypass: Bool { get set }
```

## Discussion

true if the bypass is active; otherwise, false.

## See Also

### Getting and Setting Equalizer Filter Parameters

var bandwidth: Float

The bandwidth of the equalizer filter, in octaves.

var filterType: AVAudioUnitEQFilterType

The equalizer filter type.

var frequency: Float

The frequency of the equalizer filter, in hertz.

var gain: Float

The gain of the equalizer filter, in decibels.

