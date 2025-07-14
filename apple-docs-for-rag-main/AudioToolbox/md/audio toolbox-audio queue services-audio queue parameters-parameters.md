

- Audio Toolbox
- Audio Queue Services
-  Audio Queue Parameters 

API Collection

# Audio Queue Parameters

Identifiers for audio queue parameters.

## Overview

These parameters apply only to playback audio queues. You can set a playback audio queue parameter in one of two ways:

- Set the value to take effect immediately using the AudioQueueSetParameter(_:_:_:) function.

- Schedule a value to take effect when a particular audio queue buffer plays. You supply the parameter when you enqueue the buffer. The new value is applied to the audio queue that owns the buffer when that buffer is rendered.

The AudioQueueGetParameter(_:_:_:) function always returns the current value of the parameter for an audio queue.

## Topics

### Constants

var kAudioQueueParam_Volume: AudioQueueParameterID

The playback volume for the audio queue, ranging from `0.0` through `1.0` on a linear scale. A value of `0.0` indicates silence; a value of `1.0` (the default) indicates full volume for the audio queue instance.

var kAudioQueueParam_PlayRate: AudioQueueParameterID

The playback rate for the audio queue, in the range `0.5` through `2.0`. A value of `1.0` (the default) specifies that the audio queue should play at its normal rate.

var kAudioQueueParam_Pitch: AudioQueueParameterID

The number of cents to pitch-shift the audio queue’s playback, in the range `-2400` through `2400` cents (where 1200 cents corresponds to one musical octave.)

var kAudioQueueParam_VolumeRampTime: AudioQueueParameterID

The number of seconds over which a volume change is ramped.

var kAudioQueueParam_Pan: AudioQueueParameterID

The stereo panning position of a source. For a monophonic source, panning is determined as follows:

## See Also

### Constants

typealias AudioQueuePropertyID

Identifiers for audio queue properties.

Hardware Codec Policy Keys

Indicates how an audio queue should choose between hardware and software implementations of a codec.

