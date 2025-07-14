

- AVFAudio
- AVSpeechSynthesizerDelegate
-  speechSynthesizer(\_:willSpeakRangeOfSpeechString:utterance:) 

Instance Method

# speechSynthesizer(\_:willSpeakRangeOfSpeechString:utterance:)

Tells the delegate when the synthesizer is about to speak a portion of an utterance’s text.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
optional func speechSynthesizer(
    _ synthesizer: AVSpeechSynthesizer,
    willSpeakRangeOfSpeechString characterRange: NSRange,
    utterance: AVSpeechUtterance
)
```

## Parameters 

`synthesizer`  

The speech synthesizer that’s about to speak an utterance.

`characterRange`  

The range of characters in the utterance’s speechString that correspond to the unit of speech the synthesizer is about to speak.

`utterance`  

The utterance that the speech synthesizer is about to speak.

## Discussion

The system calls this method once for each unit of speech in the utterance’s text, which is generally a word.

Tip

Implement this method if you want to provide a user interface to visually highlight each word as the synthesizer speaks it.

## See Also

### Responding to speech synthesis events

func speechSynthesizer(AVSpeechSynthesizer, didStart: AVSpeechUtterance)

Tells the delegate when the synthesizer begins speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, willSpeak: AVSpeechSynthesisMarker, utterance: AVSpeechUtterance)

Tells the delegate when the synthesizer is about to speak a marker of an utterance’s text.

func speechSynthesizer(AVSpeechSynthesizer, didPause: AVSpeechUtterance)

Tells the delegate when the synthesizer pauses while speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, didContinue: AVSpeechUtterance)

Tells the delegate when the synthesizer resumes speaking an utterance after pausing.

func speechSynthesizer(AVSpeechSynthesizer, didFinish: AVSpeechUtterance)

Tells the delegate when the synthesizer finishes speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, didCancel: AVSpeechUtterance)

Tells the delegate when the synthesizer cancels speaking an utterance.

