

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions
-  overrideMutedMicrophoneInterruption 

Type Property

# overrideMutedMicrophoneInterruption

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+watchOS 7.3+

``` source
static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions { get }
```

## Mentioned in 

Handling audio interruptions

## Discussion

Some devices include a privacy feature that mutes the built-in microphone at the hardware level in certain conditions, such as when you close the Smart Folio cover of an iPad. When this occurs, the system interrupts the audio session that’s capturing input from the microphone. Attempting to start audio input after the system mutes the microphone results in an error.

If your app uses an audio session category that supports input and output, such as playAndRecord, you can set this option to disable the default behavior and continue using the session. Disabling the default behavior may be useful to allow your app to continue playback when recording or monitoring a muted microphone doesn’t lead to a poor user experience. When you set this option, playback continues as normal, and the microphone hardware produces sample buffers, but with values of `0`.

Important

Attempting to use this option with a session category that doesn’t support audio input results in an error.

## See Also

### Getting Standard Session Options

static var mixWithOthers: AVAudioSession.CategoryOptions

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

static var duckOthers: AVAudioSession.CategoryOptions

An option that reduces the volume of other audio sessions while audio from this session plays.

static var interruptSpokenAudioAndMixWithOthers: AVAudioSession.CategoryOptions

An option that determines whether to pause spoken audio content from other sessions when your app plays its audio.

static var allowBluetooth: AVAudioSession.CategoryOptions

An option that determines whether Bluetooth hands-free devices appear as available input routes.

static var allowBluetoothA2DP: AVAudioSession.CategoryOptions

An option that determines whether you can stream audio from this session to Bluetooth devices that support the Advanced Audio Distribution Profile (A2DP).

static var allowAirPlay: AVAudioSession.CategoryOptions

An option that determines whether you can stream audio from this session to AirPlay devices.

static var defaultToSpeaker: AVAudioSession.CategoryOptions

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

