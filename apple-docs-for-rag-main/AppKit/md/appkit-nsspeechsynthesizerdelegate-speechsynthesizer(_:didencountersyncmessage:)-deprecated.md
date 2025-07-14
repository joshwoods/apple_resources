

- AppKit
- NSSpeechSynthesizerDelegate
-  speechSynthesizer(\_:didEncounterSyncMessage:) Deprecated

Instance Method

# speechSynthesizer(\_:didEncounterSyncMessage:)

Sent to the delegate when a speech synthesizer encounters a synchronization error.

macOS 10.5–14.0Deprecated

``` source
@MainActor
optional func speechSynthesizer(
    _ sender: NSSpeechSynthesizer,
    didEncounterSyncMessage message: String
)
```

## Parameters 

`sender`  

Speech synthesizer informing its delegate of an error.

`message`  

Error message.

## Discussion

The synthesizer calls your synchronization delegate method whenever it encounters a synchronization command embedded in a string. You might use the synchronization delegate method to provide a callback not ordinarily provided.

For example, you might insert synchronization commands at the end of every sentence in a string, or you might enter synchronization commands after every numeric value in the text.

However, to synchronize your application with phonemes or words, it makes more sense to use the built-in phoneme and word delegate methods: speechSynthesizer(_:willSpeakPhoneme:) and speechSynthesizer(_:willSpeakWord:of:).

## See Also

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

func speechSynthesizer(NSSpeechSynthesizer, didFinishSpeaking: Bool)

Sent when an NSSpeechSynthesizer object finishes speaking through the sound output device.

Deprecated

