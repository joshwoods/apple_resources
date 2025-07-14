

- AVFAudio
- AVSpeechSynthesizer
-  mixToTelephonyUplink 

Instance Property

# mixToTelephonyUplink

A Boolean value that specifies whether to send synthesized speech to an active call.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 6.0+

``` source
var mixToTelephonyUplink: Bool { get set }
```

## Discussion

This property has no effect when there isn’t an active call.

## See Also

### Directing speech output

var usesApplicationAudioSession: Bool

A Boolean value that specifies whether the app manages the audio session.

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

