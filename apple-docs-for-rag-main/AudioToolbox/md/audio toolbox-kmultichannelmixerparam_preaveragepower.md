

- Audio Toolbox
-  kMultiChannelMixerParam_PreAveragePower 

Global Variable

# kMultiChannelMixerParam_PreAveragePower

The average power level of the channel, prior to the mixer, in decibels.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kMultiChannelMixerParam_PreAveragePower: AudioUnitParameterID { get }
```

## Discussion

Input and output scope. This is a read-only property. Use the value of this constant to read the left channel and its value+1 to read the right channel.

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

var kMultiChannelMixerParam_PrePeakHoldLevel: AudioUnitParameterID

The peak hold level of the channel, prior to the mixer, in decibels.

var kMultiChannelMixerParam_Volume: AudioUnitParameterID

The linear gain of the channel.

