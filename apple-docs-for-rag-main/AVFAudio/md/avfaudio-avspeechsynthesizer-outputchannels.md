

- AVFAudio
- AVSpeechSynthesizer
-  outputChannels 

Instance Property

# outputChannels

An array of audio session channels to route generated speech.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var outputChannels: [AVAudioSessionChannelDescription]? { get set }
```

## Discussion

The system replicates speech audio to each audio session channel.

## See Also

### Directing speech output

var usesApplicationAudioSession: Bool

A Boolean value that specifies whether the app manages the audio session.

var mixToTelephonyUplink: Bool

A Boolean value that specifies whether to send synthesized speech to an active call.

func write(AVSpeechUtterance, toBufferCallback: AVSpeechSynthesizer.BufferCallback)

Generates speech for the utterance and invokes the callback with the audio buffer.

typealias BufferCallback

A type that defines a callback that receives a buffer of generated speech.

func write(AVSpeechUtterance, toBufferCallback: AVSpeechSynthesizer.BufferCallback, toMarkerCallback: AVSpeechSynthesizer.MarkerCallback)

Generates audio buffers and associated metadata for storage or further speech synthesis processing.

typealias MarkerCallback

A type that defines a callback that receives speech markers.

