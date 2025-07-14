

- Audio Toolbox
-  kAudioSessionProperty_OverrideAudioRoute 

Global Variable

# kAudioSessionProperty_OverrideAudioRoute

Specifies whether or not to override the audio session category’s typical audio route.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionProperty_OverrideAudioRoute: Int { get }
```

## Discussion

A write-only `UInt32` value. Can be set with one of two values: kAudioSessionOverrideAudioRoute_None, which specifies that you want to use the typical audio route; and kAudioSessionOverrideAudioRoute_Speaker, when sends output audio to the built-in speaker. This property can be used only with the kAudioSessionCategory_PlayAndRecord (or the equivalent playAndRecord) category.

If a headset is plugged in at the time you set this property’s value to kAudioSessionOverrideAudioRoute_Speaker, the system changes the audio routing for input as well as for output: input comes from the built-in microphone; output goes to the built-in speaker.

Upon an audio route change (such as by plugging in or unplugging a headset), or upon interruption, this property reverts to its default value.

See also kAudioSessionProperty_OverrideCategoryDefaultToSpeaker.

## See Also

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

var kAudioSessionProperty_AudioInputAvailable: Int

Indicates if audio input is available (a nonzero value) or not (a value of 0).

var kAudioSessionProperty_ServerDied: Int

Indicates if the audio server has died (indicated by a nonzero `UInt32` value) or is still running (a value of 0).

var kAudioSessionProperty_OtherMixableAudioShouldDuck: Int

For audio session categories that allow audio mixing with other apps, specifies whether other audio should be reduced in level when your app produces sound. This property has a value of `FALSE` (0) by default. Set it to a nonzero value to turn on ducking.

