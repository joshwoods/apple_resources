

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions
-  allowBluetooth 

Type Property

# allowBluetooth

An option that determines whether Bluetooth hands-free devices appear as available input routes.

iOSiPadOSMac CatalysttvOS 17.0+visionOSwatchOS 11.0+

``` source
static var allowBluetooth: AVAudioSession.CategoryOptions { get }
```

## Discussion

You’re required to set this option to allow routing audio input and output to a paired Bluetooth Hands-Free Profile (HFP) device. If you clear this option, paired Bluetooth HFP devices don’t show up as available audio input routes.

If an application uses the setPreferredInput(_:) method to select a Bluetooth HFP input, the output automatically changes to the corresponding Bluetooth HFP output. Likewise, selecting a Bluetooth HFP output using an MPVolumeView object’s route picker automatically changes the input to the corresponding Bluetooth HFP input. Therefore, both audio input and output are routed to the Bluetooth HFP device even though you only selected the input or output.

You can set this option only if the audio session category is playAndRecord or record.

## See Also

### Getting Standard Session Options

static var mixWithOthers: AVAudioSession.CategoryOptions

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

static var duckOthers: AVAudioSession.CategoryOptions

An option that reduces the volume of other audio sessions while audio from this session plays.

static var interruptSpokenAudioAndMixWithOthers: AVAudioSession.CategoryOptions

An option that determines whether to pause spoken audio content from other sessions when your app plays its audio.

static var allowBluetoothA2DP: AVAudioSession.CategoryOptions

An option that determines whether you can stream audio from this session to Bluetooth devices that support the Advanced Audio Distribution Profile (A2DP).

static var allowAirPlay: AVAudioSession.CategoryOptions

An option that determines whether you can stream audio from this session to AirPlay devices.

static var defaultToSpeaker: AVAudioSession.CategoryOptions

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

