

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions
-  allowAirPlay 

Type Property

# allowAirPlay

An option that determines whether you can stream audio from this session to AirPlay devices.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
static var allowAirPlay: AVAudioSession.CategoryOptions { get }
```

## Discussion

Setting this option enables the audio session to route audio output to AirPlay devices. You can only explicitly set this option if the audio session’s category is set to playAndRecord. For most other audio session categories, the system sets this option implicitly.

Audio sessions using the multiRoute or record categories implicitly clear this option.

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

static var defaultToSpeaker: AVAudioSession.CategoryOptions

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

