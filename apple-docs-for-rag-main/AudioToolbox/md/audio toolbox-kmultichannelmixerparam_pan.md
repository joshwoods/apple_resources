

- Audio Toolbox
-  kMultiChannelMixerParam_Pan 

Global Variable

# kMultiChannelMixerParam_Pan

The panning value for the mixer.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kMultiChannelMixerParam_Pan: AudioUnitParameterID { get }
```

## Discussion

Global scope. The value should be a number between `-1.0` and `1.0`, where `-1.0` represents far left and `1.0` represents far right. The default value is `0`. Setting kAudioUnitProperty_MatrixLevels overrides any value set for `kMultiChannelMixerParam_Pan` and vice versa.

## See Also

### Constants

var kMultiChannelMixerParam_Enable: AudioUnitParameterID

Enables a channel.

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

