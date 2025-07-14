

- AppKit
- NSSpeechSynthesizerDelegate
-  speechSynthesizer(\_:willSpeakWord:of:) Deprecated

Instance Method

# speechSynthesizer(\_:willSpeakWord:of:)

Sent just before a synthesized word is spoken through the sound output device.

macOS 10.3–14.0Deprecated

``` source
@MainActor
optional func speechSynthesizer(
    _ sender: NSSpeechSynthesizer,
    willSpeakWord characterRange: NSRange,
    of string: String
)
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Parameters 

`sender`  

An NSSpeechSynthesizer object that’s synthesizing text into speech.

`characterRange`  

Word that `sender` is about to speak into the sound output device.

`string`  

Text that is being synthesized by `sender`.

## Discussion

One use of this method might be to visually highlight the word being spoken.

Important

In OS X v10.4 and earlier, the delegate is not sent this message when the `NSSpeechSynthesizer` object is synthesizing speech to a file (startSpeaking(_:to:)).

## See Also

### Related Documentation

func startSpeaking(String) -> Bool

Begins speaking synthesized text through the system’s default sound output device.

Deprecated

Speech Programming Topics

### Synthesizing Speech

func speechSynthesizer(NSSpeechSynthesizer, willSpeakPhoneme: Int16)

Sent just before a synthesized phoneme is spoken through the sound output device.

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

