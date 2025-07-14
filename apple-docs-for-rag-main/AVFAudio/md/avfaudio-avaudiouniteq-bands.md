

- AVFAudio
- AVAudioUnitEQ
-  bands 

Instance Property

# bands

An array of equalizer filter parameters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var bands: [AVAudioUnitEQFilterParameters] { get }
```

## Discussion

The number of elements in the array is equal to the number of bands.

## See Also

### Getting and setting the equalizer values

class AVAudioUnitEQFilterParameters

An object that encapsulates the parameters that the equalizer uses.

var globalGain: Float

The overall gain adjustment that the audio unit applies to the signal, in decibels.

