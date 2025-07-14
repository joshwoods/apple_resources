

- AVFAudio
- AVSpeechSynthesizerDelegate
-  speechSynthesizer(\_:didContinue:) 

Instance Method

# speechSynthesizer(\_:didContinue:)

Tells the delegate when the synthesizer resumes speaking an utterance after pausing.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
optional func speechSynthesizer(
    _ synthesizer: AVSpeechSynthesizer,
    didContinue utterance: AVSpeechUtterance
)
```

## Parameters 

`synthesizer`  

The speech synthesizer that resumes speaking the utterance.

`utterance`  

The utterance that the speech synthesizer resumes speaking.

## Discussion

The system only calls this method if a speech synthesizer pauses speaking and the system calls its pauseSpeaking(at:) method. The system doesn’t call this method if the synthesizer pauses while in a delay between utterances.

## See Also

### Responding to speech synthesis events

func speechSynthesizer(AVSpeechSynthesizer, didStart: AVSpeechUtterance)

Tells the delegate when the synthesizer begins speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, willSpeakRangeOfSpeechString: NSRange, utterance: AVSpeechUtterance)

Tells the delegate when the synthesizer is about to speak a portion of an utterance’s text.

func speechSynthesizer(AVSpeechSynthesizer, willSpeak: AVSpeechSynthesisMarker, utterance: AVSpeechUtterance)

Tells the delegate when the synthesizer is about to speak a marker of an utterance’s text.

func speechSynthesizer(AVSpeechSynthesizer, didPause: AVSpeechUtterance)

Tells the delegate when the synthesizer pauses while speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, didFinish: AVSpeechUtterance)

Tells the delegate when the synthesizer finishes speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, didCancel: AVSpeechUtterance)

Tells the delegate when the synthesizer cancels speaking an utterance.

