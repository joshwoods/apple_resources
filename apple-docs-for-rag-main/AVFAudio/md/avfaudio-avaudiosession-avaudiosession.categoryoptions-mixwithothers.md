

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions
-  mixWithOthers 

Type Property

# mixWithOthers

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
static var mixWithOthers: AVAudioSession.CategoryOptions { get }
```

## Discussion

You can set this option explicitly only if the audio session category is playAndRecord, playback, or multiRoute. If you set the audio session category to ambient, the session automatically sets this option. Likewise, setting the duckOthers or interruptSpokenAudioAndMixWithOthers options also enables this option.

Clearing this option and then activating your session interrupts other audio sessions. If you set this option, your app mixes its audio with audio playing in background apps, such as the Music app.

## See Also

### Getting Standard Session Options

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

static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

