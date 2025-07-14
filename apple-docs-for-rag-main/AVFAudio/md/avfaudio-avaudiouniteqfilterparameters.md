

- AVFAudio
-  AVAudioUnitEQFilterParameters 

Class

# AVAudioUnitEQFilterParameters

An object that encapsulates the parameters that the equalizer uses.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioUnitEQFilterParameters
```

## Overview

Note

Don’t create an instance of the `AVAudioUnitEQFilterParameters` class directly. Use the array that returns from the bands property of AVAudioUnitEQ.

## Topics

### Getting and Setting Equalizer Filter Parameters

var bandwidth: Float

The bandwidth of the equalizer filter, in octaves.

var bypass: Bool

The bypass state of the equalizer filter band.

var filterType: AVAudioUnitEQFilterType

The equalizer filter type.

var frequency: Float

The frequency of the equalizer filter, in hertz.

var gain: Float

The gain of the equalizer filter, in decibels.

### Constants

enum AVAudioUnitEQFilterType

Filter types available to use with the filter type property.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Getting and setting the equalizer values

var bands: [AVAudioUnitEQFilterParameters]

An array of equalizer filter parameters.

var globalGain: Float

The overall gain adjustment that the audio unit applies to the signal, in decibels.

