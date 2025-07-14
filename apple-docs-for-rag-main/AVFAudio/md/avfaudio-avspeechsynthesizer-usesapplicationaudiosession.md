

- AVFAudio
- AVSpeechSynthesizer
-  usesApplicationAudioSession 

Instance Property

# usesApplicationAudioSession

A Boolean value that specifies whether the app manages the audio session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var usesApplicationAudioSession: Bool { get set }
```

## Discussion

If you set this value to false, the system creates a separate audio session to automatically manage speech, interruptions, and mixing and ducking the speech with other audio sources.

## See Also

### Directing speech output

var mixToTelephonyUplink: Bool

A Boolean value that specifies whether to send synthesized speech to an active call.

var outputChannels: [AVAudioSessionChannelDescription]?

An array of audio session channels to route generated speech.

func write(AVSpeechUtterance, toBufferCallback: AVSpeechSynthesizer.BufferCallback)

Generates speech for the utterance and invokes the callback with the audio buffer.

typealias BufferCallback

A type that defines a callback that receives a buffer of generated speech.

func write(AVSpeechUtterance, toBufferCallback: AVSpeechSynthesizer.BufferCallback, toMarkerCallback: AVSpeechSynthesizer.MarkerCallback)

Generates audio buffers and associated metadata for storage or further speech synthesis processing.

typealias MarkerCallback

A type that defines a callback that receives speech markers.

