

- AVFAudio
- AVSpeechSynthesizer
-  write(\_:toBufferCallback:toMarkerCallback:) 

Instance Method

# write(\_:toBufferCallback:toMarkerCallback:)

Generates audio buffers and associated metadata for storage or further speech synthesis processing.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func write(
    _ utterance: AVSpeechUtterance,
    toBufferCallback bufferCallback: @escaping AVSpeechSynthesizer.BufferCallback,
    toMarkerCallback markerCallback: @escaping AVSpeechSynthesizer.MarkerCallback
)
```

## Parameters 

`utterance`  

A utterance for a synthesizer to speak.

`bufferCallback`  

A callback that the system invokes with the synthesized audio data.

`markerCallback`  

A callback that the system invokes with marker information.

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

typealias BufferCallback

A type that defines a callback that receives a buffer of generated speech.

typealias MarkerCallback

A type that defines a callback that receives speech markers.

