

- AppKit
- NSSpeechSynthesizerDelegate
-  speechSynthesizer(\_:didEncounterErrorAt:of:message:) Deprecated

Instance Method

# speechSynthesizer(\_:didEncounterErrorAt:of:message:)

Sent to the delegate when a speech synthesizer encounters an error in text being synthesized.

macOS 10.5–14.0Deprecated

``` source
@MainActor
optional func speechSynthesizer(
    _ sender: NSSpeechSynthesizer,
    didEncounterErrorAt characterIndex: Int,
    of string: String,
    message: String
)
```

## Parameters 

`sender`  

Speech synthesizer informing its delegate of an error.

`characterIndex`  

Location in text where the receiver encountered the error.

`string`  

Text the receiver was synthesizing when the error occurred.

`message`  

Error message.

## Discussion

The synthesizer sends an error delegate message whenever it encounters a syntax error within a command embedded in the string it is processing. This can be useful during application debugging, to detect problems with commands that you have embedded in strings that your application speaks. It can also be useful if your application allows users to embed commands within strings. Your application might display an alert indicating that the synthesizer encountered a problem in processing an embedded command.

If your application needs information about errors that occurred prior to calling your error delegate method, the application (including the error delegate method) can call the sender’s object(forProperty:) method with the errors constant.

## See Also

### Synthesizing Speech

func speechSynthesizer(NSSpeechSynthesizer, willSpeakWord: NSRange, of: String)

Sent just before a synthesized word is spoken through the sound output device.

Deprecated

func speechSynthesizer(NSSpeechSynthesizer, willSpeakPhoneme: Int16)

Sent just before a synthesized phoneme is spoken through the sound output device.

Deprecated

func speechSynthesizer(NSSpeechSynthesizer, didEncounterSyncMessage: String)

Sent to the delegate when a speech synthesizer encounters a synchronization error.

Deprecated

func speechSynthesizer(NSSpeechSynthesizer, didFinishSpeaking: Bool)

Sent when an NSSpeechSynthesizer object finishes speaking through the sound output device.

Deprecated

