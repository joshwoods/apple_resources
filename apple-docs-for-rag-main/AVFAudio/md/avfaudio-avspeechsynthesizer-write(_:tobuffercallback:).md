

- AVFAudio
- AVSpeechSynthesizer
-  write(\_:toBufferCallback:) 

Instance Method

# write(\_:toBufferCallback:)

Generates speech for the utterance and invokes the callback with the audio buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func write(
    _ utterance: AVSpeechUtterance,
    toBufferCallback bufferCallback: @escaping AVSpeechSynthesizer.BufferCallback
)
```

## Parameters 

`utterance`  

The utterance for synthesizing speech.

`bufferCallback`  

The system calls this closure with the generated audio buffer.

## Discussion

Call this method to receive audio buffers to store or further process synthesized speech.

## See Also

### Directing speech output

var usesApplicationAudioSession: Bool

A Boolean value that specifies whether the app manages the audio session.

var mixToTelephonyUplink: Bool

A Boolean value that specifies whether to send synthesized speech to an active call.

var outputChannels: [AVAudioSessionChannelDescription]?

An array of audio session channels to route generated speech.

typealias BufferCallback

A type that defines a callback that receives a buffer of generated speech.

func write(AVSpeechUtterance, toBufferCallback: AVSpeechSynthesizer.BufferCallback, toMarkerCallback: AVSpeechSynthesizer.MarkerCallback)

Generates audio buffers and associated metadata for storage or further speech synthesis processing.

typealias MarkerCallback

A type that defines a callback that receives speech markers.

