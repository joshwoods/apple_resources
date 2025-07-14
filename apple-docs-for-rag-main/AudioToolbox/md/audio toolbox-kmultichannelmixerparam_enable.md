

- Audio Toolbox
-  kMultiChannelMixerParam_Enable 

Global Variable

# kMultiChannelMixerParam_Enable

Enables a channel.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kMultiChannelMixerParam_Enable: AudioUnitParameterID { get }
```

## Discussion

Global scope. The value is a boolean: use `0` to disable the channel or `1` to enable the channel. The default value is `1`.

## See Also

### Constants

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

var kMultiChannelMixerParam_Volume: AudioUnitParameterID

The linear gain of the channel.

