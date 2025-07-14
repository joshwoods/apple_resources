

- Audio Toolbox
-  kMultiChannelMixerParam_Volume 

Global Variable

# kMultiChannelMixerParam_Volume

The linear gain of the channel.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kMultiChannelMixerParam_Volume: AudioUnitParameterID { get }
```

## Discussion

Global scope. The value should be a number between `0.0` and `1.0`. The default value is `1.0`.

## See Also

### Constants

var kMultiChannelMixerParam_Enable: AudioUnitParameterID

Enables a channel.

var kMultiChannelMixerParam_Pan: AudioUnitParameterID

The panning value for the mixer.

var kMultiChannelMixerParam_PostAveragePower: AudioUnitParameterID

The average power level of the channel, after the mixer, in decibels.

var kMultiChannelMixerParam_PostPeakHoldLevel: AudioUnitParameterID

The peak hold level of the channel, after the mixer, in decibels.

var kMultiChannelMixerParam_PreAveragePower: AudioUnitParameterID

The average power level of the channel, prior to the mixer, in decibels.

var kMultiChannelMixerParam_PrePeakHoldLevel: AudioUnitParameterID

The peak hold level of the channel, prior to the mixer, in decibels.

