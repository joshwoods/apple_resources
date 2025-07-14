

- AppKit
- NSSpeechSynthesizerDelegate
-  speechSynthesizer(\_:didFinishSpeaking:) Deprecated

Instance Method

# speechSynthesizer(\_:didFinishSpeaking:)

Sent when an NSSpeechSynthesizer object finishes speaking through the sound output device.

macOS 10.3–14.0Deprecated

``` source
@MainActor
optional func speechSynthesizer(
    _ sender: NSSpeechSynthesizer,
    didFinishSpeaking finishedSpeaking: Bool
)
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Parameters 

`sender`  

An NSSpeechSynthesizer object that has stopped speaking into the sound output device.

`finishedSpeaking`  

true when speaking completed normally, false if speaking is stopped prematurely for any reason.

## See Also

### Related Documentation

func startSpeaking(String) -> Bool

Begins speaking synthesized text through the system’s default sound output device.

Deprecated

func stopSpeaking()

Stops synthesis in progress.

Deprecated

### Synthesizing Speech

func speechSynthesizer(NSSpeechSynthesizer, willSpeakWord: NSRange, of: String)

Sent just before a synthesized word is spoken through the sound output device.

Deprecated

func speechSynthesizer(NSSpeechSynthesizer, willSpeakPhoneme: Int16)

Sent just before a synthesized phoneme is spoken through the sound output device.

Deprecated

func speechSynthesizer(NSSpeechSynthesizer, didEncounterErrorAt: Int, of: String, message: String)

Sent to the delegate when a speech synthesizer encounters an error in text being synthesized.

Deprecated

func speechSynthesizer(NSSpeechSynthesizer, didEncounterSyncMessage: String)

Sent to the delegate when a speech synthesizer encounters a synchronization error.

Deprecated

