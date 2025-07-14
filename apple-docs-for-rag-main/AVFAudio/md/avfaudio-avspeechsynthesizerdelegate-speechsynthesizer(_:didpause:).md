

- AVFAudio
- AVSpeechSynthesizerDelegate
-  speechSynthesizer(\_:didPause:) 

Instance Method

# speechSynthesizer(\_:didPause:)

Tells the delegate when the synthesizer pauses while speaking an utterance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
optional func speechSynthesizer(
    _ synthesizer: AVSpeechSynthesizer,
    didPause utterance: AVSpeechUtterance
)
```

## Parameters 

`synthesizer`  

The speech synthesizer that pauses speaking the utterance.

`utterance`  

The utterance that the speech synthesizer pauses speaking.

## Discussion

The system only calls this method if a speech synthesizer is speaking an utterance and the system calls its pauseSpeaking(at:) method. The system doesn’t call this method if the synthesizer is in a delay between utterances when speech pauses.

## See Also

### Responding to speech synthesis events

func speechSynthesizer(AVSpeechSynthesizer, didStart: AVSpeechUtterance)

Tells the delegate when the synthesizer begins speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, willSpeakRangeOfSpeechString: NSRange, utterance: AVSpeechUtterance)

Tells the delegate when the synthesizer is about to speak a portion of an utterance’s text.

func speechSynthesizer(AVSpeechSynthesizer, willSpeak: AVSpeechSynthesisMarker, utterance: AVSpeechUtterance)

Tells the delegate when the synthesizer is about to speak a marker of an utterance’s text.

func speechSynthesizer(AVSpeechSynthesizer, didContinue: AVSpeechUtterance)

Tells the delegate when the synthesizer resumes speaking an utterance after pausing.

func speechSynthesizer(AVSpeechSynthesizer, didFinish: AVSpeechUtterance)

Tells the delegate when the synthesizer finishes speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, didCancel: AVSpeechUtterance)

Tells the delegate when the synthesizer cancels speaking an utterance.

