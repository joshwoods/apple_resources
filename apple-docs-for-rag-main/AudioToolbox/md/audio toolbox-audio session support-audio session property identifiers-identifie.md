

- Audio Toolbox
- Audio Session Support
-  Audio Session Property Identifiers 

API Collection

# Audio Session Property Identifiers

Property identifiers used with Audio Session Services in iOS.

## Overview

Use these property identifiers in concert with the AudioSessionGetProperty(_:_:_:), AudioSessionSetProperty(_:_:_:), and AudioSessionAddPropertyListener(_:_:_:) functions.

## Topics

### Constants

var kAudioSessionProperty_PreferredHardwareSampleRate: Int

Your preferred hardware sample rate for the audio session. A read/write `Float64` value. The actual sample rate may be different and can be obtained using the `kAudioSessionProperty_CurrentHardwareSampleRate` property.

Deprecated

var kAudioSessionProperty_PreferredHardwareIOBufferDuration: Int

Your preferred hardware I/O buffer duration in seconds. Do not set this property unless you require lower I/O latency than is provided by default.

var kAudioSessionProperty_AudioCategory: Int

The category for the audio session. A read/write `UInt32` value.

var kAudioSessionProperty_AudioRouteChange: Int

The reason the audio route changed.

var kAudioSessionProperty_CurrentHardwareSampleRate: Int

Indicates the current hardware sample rate. A read-only `Float64` value.

var kAudioSessionProperty_CurrentHardwareInputNumberChannels: Int

Indicates the current number of audio hardware input channels. A read-only `UInt32` value.

var kAudioSessionProperty_CurrentHardwareOutputNumberChannels: Int

Indicates the current number of audio hardware output channels. A read-only `UInt32` value.

var kAudioSessionProperty_CurrentHardwareOutputVolume: Int

Indicates the current audio output volume as `Float32` value between 0.0 and 1.0. Read-only. This value is available to your app by way of a property listener callback function. See AudioSessionAddPropertyListener(_:_:_:).

var kAudioSessionProperty_CurrentHardwareInputLatency: Int

Indicates the current hardware input latency, in seconds, as a read-only `Float32` value.

var kAudioSessionProperty_CurrentHardwareOutputLatency: Int

Indicates the current hardware output latency, in seconds, as a read-only `Float32` value.

var kAudioSessionProperty_CurrentHardwareIOBufferDuration: Int

Indicates the current hardware IO buffer duration, in seconds, as a read-only `Float32` value.

var kAudioSessionProperty_OtherAudioIsPlaying: Int

Indicates whether or not another app (typically, the iPod app) is currently playing audio. Read-only. A non-zero `UInt32` value indicates that other audio is playing.

var kAudioSessionProperty_OverrideAudioRoute: Int

Specifies whether or not to override the audio session category’s typical audio route.

var kAudioSessionProperty_AudioInputAvailable: Int

Indicates if audio input is available (a nonzero value) or not (a value of 0).

var kAudioSessionProperty_ServerDied: Int

Indicates if the audio server has died (indicated by a nonzero `UInt32` value) or is still running (a value of 0).

var kAudioSessionProperty_OtherMixableAudioShouldDuck: Int

For audio session categories that allow audio mixing with other apps, specifies whether other audio should be reduced in level when your app produces sound. This property has a value of `FALSE` (0) by default. Set it to a nonzero value to turn on ducking.

var kAudioSessionProperty_OverrideCategoryMixWithOthers: Int

Changes the mixing behavior of the kAudioSessionCategory_MediaPlayback and kAudioSessionCategory_PlayAndRecord audio session categories.

var kAudioSessionProperty_OverrideCategoryDefaultToSpeaker: Int

Specifies whether or not to route audio to the speaker (instead of to the receiver) when no other audio route, such as a headset, is connected.

var kAudioSessionProperty_OverrideCategoryEnableBluetoothInput: Int

Allows a paired Bluetooth device to appear as an available audio input route.

var kAudioSessionProperty_InterruptionType: Int

Indicates the type of an end-interruption event.

var kAudioSessionProperty_Mode: Int

A read/write `UIInt32` value that specifies the audio session mode.

var kAudioSessionProperty_InputSources: Int

Details on the available audio input sources.

var kAudioSessionProperty_OutputDestinations: Int

Details on the available audio output destinations.

var kAudioSessionProperty_InputSource: Int

The audio input source.

var kAudioSessionProperty_OutputDestination: Int

The audio output destination.

var kAudioSessionProperty_InputGainAvailable: Int

A read-only `UInt32` value that indicates whether or not audio input gain adjustment is available, where a nonzero value means adjustment is available.

var kAudioSessionProperty_InputGainScalar: Int

A read/write `Float32` value that indicates the audio input gain setting for the active input source.

var kAudioSessionProperty_AudioRouteDescription: Int

Information about an audio route.

## See Also

### Audio Session Support

Audio Session Categories

Category identifiers for audio sessions, used as values for the kAudioSessionProperty_AudioCategory property.

Audio Session Modes

Mode identifiers for audio sessions, used as values for the kAudioSessionProperty_Mode property.

Audio Session Category Route Overrides

Specifies whether the default audio route for the `PlayAndRecord` category should be overridden.

Audio Session Activation Flags

Flags that provide additional information about your app’s audio intentions upon session activation or deactivation.

Audio Session Interruption States

Identifiers used with the AudioSessionInterruptionListener callback function in iOS to indicate that an audio interruption has started or stopped.

typealias AudioSessionInterruptionType

Values that indicate the nature of the interruption that ended.

