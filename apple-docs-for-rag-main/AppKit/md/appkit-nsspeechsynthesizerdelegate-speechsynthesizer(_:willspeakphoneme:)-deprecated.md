

- AppKit
- NSSpeechSynthesizerDelegate
-  speechSynthesizer(\_:willSpeakPhoneme:) Deprecated

Instance Method

# speechSynthesizer(\_:willSpeakPhoneme:)

Sent just before a synthesized phoneme is spoken through the sound output device.

macOS 10.3–14.0Deprecated

``` source
@MainActor
optional func speechSynthesizer(
    _ sender: NSSpeechSynthesizer,
    willSpeakPhoneme phonemeOpcode: Int16
)
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Parameters 

`sender`  

An NSSpeechSynthesizer object that’s synthesizing text into speech.

`phonemeOpcode`  

Phoneme that `sender` is about to speak into the sound output device.

## Discussion

One use of this method might be to animate a mouth on screen to match the generated speech.

### Special Considerations

This method is not sent for modern voices. It is only supported for MacinTalk voices.

In OS X v10.4 and earlier, the delegate is not sent this message when the `NSSpeechSynthesizer` object is synthesizing speech to a file (startSpeaking(_:to:)).

## See Also

### Related Documentation

func startSpeaking(String) -> Bool

Begins speaking synthesized text through the system’s default sound output device.

Deprecated

### Synthesizing Speech

func speechSynthesizer(NSSpeechSynthesizer, willSpeakWord: NSRange, of: String)

Sent just before a synthesized word is spoken through the sound output device.

Deprecated

func speechSynthesizer(NSSpeechSynthesizer, didEncounterErrorAt: Int, of: String, message: String)

Sent to the delegate when a speech synthesizer encounters an error in text being synthesized.

Deprecated

func speechSynthesizer(NSSpeechSynthesizer, didEncounterSyncMessage: String)

Sent to the delegate when a speech synthesizer encounters a synchronization error.

Deprecated

func speechSynthesizer(NSSpeechSynthesizer, didFinishSpeaking: Bool)

Sent when an NSSpeechSynthesizer object finishes speaking through the sound output device.

Deprecated

