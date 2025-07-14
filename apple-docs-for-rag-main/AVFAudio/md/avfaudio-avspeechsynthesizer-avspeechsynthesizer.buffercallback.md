

- AVFAudio
- AVSpeechSynthesizer
-  AVSpeechSynthesizer.BufferCallback 

Type Alias

# AVSpeechSynthesizer.BufferCallback

A type that defines a callback that receives a buffer of generated speech.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias BufferCallback = (AVAudioBuffer) -> Void
```

## See Also

### Directing speech output

var usesApplicationAudioSession: Bool

A Boolean value that specifies whether the app manages the audio session.

var mixToTelephonyUplink: Bool

A Boolean value that specifies whether to send synthesized speech to an active call.

var outputChannels: [AVAudioSessionChannelDescription]?

An array of audio session channels to route generated speech.

func write(AVSpeechUtterance, toBufferCallback: AVSpeechSynthesizer.BufferCallback)

Generates speech for the utterance and invokes the callback with the audio buffer.

func write(AVSpeechUtterance, toBufferCallback: AVSpeechSynthesizer.BufferCallback, toMarkerCallback: AVSpeechSynthesizer.MarkerCallback)

Generates audio buffers and associated metadata for storage or further speech synthesis processing.

typealias MarkerCallback

A type that defines a callback that receives speech markers.

