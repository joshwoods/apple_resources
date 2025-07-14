

- Audio Toolbox
-  kAudioSessionProperty_OverrideCategoryDefaultToSpeaker 

Global Variable

# kAudioSessionProperty_OverrideCategoryDefaultToSpeaker

Specifies whether or not to route audio to the speaker (instead of to the receiver) when no other audio route, such as a headset, is connected.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionProperty_OverrideCategoryDefaultToSpeaker: Int { get }
```

## Discussion

A read/write `UInt32` value. By default, the value of this property is `FALSE` (`0`).

This property retains its value through an audio route change (such as when plugging in or unplugging a headset), and upon interruption; it reverts to its default value only upon an audio session category change. This property can be used only with the kAudioSessionCategory_PlayAndRecord (or the equivalent playAndRecord) category.

See also kAudioSessionProperty_OverrideAudioRoute.

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

var kAudioSessionProperty_OverrideAudioRoute: Int

Specifies whether or not to override the audio session category’s typical audio route.

var kAudioSessionProperty_AudioInputAvailable: Int

Indicates if audio input is available (a nonzero value) or not (a value of 0).

var kAudioSessionProperty_ServerDied: Int

Indicates if the audio server has died (indicated by a nonzero `UInt32` value) or is still running (a value of 0).

