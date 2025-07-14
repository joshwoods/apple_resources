

- AVFAudio
- AVSpeechSynthesizerDelegate
-  speechSynthesizer(\_:willSpeak:utterance:) 

Instance Method

# speechSynthesizer(\_:willSpeak:utterance:)

Tells the delegate when the synthesizer is about to speak a marker of an utterance’s text.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
optional func speechSynthesizer(
    _ synthesizer: AVSpeechSynthesizer,
    willSpeak marker: AVSpeechSynthesisMarker,
    utterance: AVSpeechUtterance
)
```

## Parameters 

`synthesizer`  

The speech synthesizer that’s about to speak a marker of an utterance.

`marker`  

The synthesized audio that the speech synthesizer is about to speak.

`utterance`  

The utterance that the speech synthesizer pauses speaking.

## See Also

### Responding to speech synthesis events

func speechSynthesizer(AVSpeechSynthesizer, didStart: AVSpeechUtterance)

Tells the delegate when the synthesizer begins speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, willSpeakRangeOfSpeechString: NSRange, utterance: AVSpeechUtterance)

Tells the delegate when the synthesizer is about to speak a portion of an utterance’s text.

func speechSynthesizer(AVSpeechSynthesizer, didPause: AVSpeechUtterance)

Tells the delegate when the synthesizer pauses while speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, didContinue: AVSpeechUtterance)

Tells the delegate when the synthesizer resumes speaking an utterance after pausing.

func speechSynthesizer(AVSpeechSynthesizer, didFinish: AVSpeechUtterance)

Tells the delegate when the synthesizer finishes speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, didCancel: AVSpeechUtterance)

Tells the delegate when the synthesizer cancels speaking an utterance.

