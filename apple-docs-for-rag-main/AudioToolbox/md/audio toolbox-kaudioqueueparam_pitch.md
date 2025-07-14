

- Audio Toolbox
-  kAudioQueueParam_Pitch 

Global Variable

# kAudioQueueParam_Pitch

The number of cents to pitch-shift the audio queue’s playback, in the range `-2400` through `2400` cents (where 1200 cents corresponds to one musical octave.)

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioQueueParam_Pitch: AudioQueueParameterID { get }
```

## Discussion

This parameter is usable only if the time/pitch processor is enabled.

## See Also

### Constants

var kAudioQueueParam_Volume: AudioQueueParameterID

The playback volume for the audio queue, ranging from `0.0` through `1.0` on a linear scale. A value of `0.0` indicates silence; a value of `1.0` (the default) indicates full volume for the audio queue instance.

var kAudioQueueParam_PlayRate: AudioQueueParameterID

The playback rate for the audio queue, in the range `0.5` through `2.0`. A value of `1.0` (the default) specifies that the audio queue should play at its normal rate.

var kAudioQueueParam_VolumeRampTime: AudioQueueParameterID

The number of seconds over which a volume change is ramped.

var kAudioQueueParam_Pan: AudioQueueParameterID

The stereo panning position of a source. For a monophonic source, panning is determined as follows:

