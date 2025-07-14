

- AVFAudio
-  AVSpeechSynthesizerDelegate 

Protocol

# AVSpeechSynthesizerDelegate

A delegate protocol that contains optional methods you can implement to respond to events that occur during speech synthesis.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol AVSpeechSynthesizerDelegate : NSObjectProtocol, Sendable
```

## Overview

A speech synthesizer sends messages to its delegate for three categories of events:

- The synthesizer starts or finishes speaking an utterance.

- Speech pauses or resumes.

- The synthesizer produces each individual unit of speech, which is generally a word.

## Topics

### Responding to speech synthesis events

func speechSynthesizer(AVSpeechSynthesizer, didStart: AVSpeechUtterance)

Tells the delegate when the synthesizer begins speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, willSpeakRangeOfSpeechString: NSRange, utterance: AVSpeechUtterance)

Tells the delegate when the synthesizer is about to speak a portion of an utterance’s text.

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

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

## See Also

### Managing the delegate

var delegate: (any AVSpeechSynthesizerDelegate)?

The delegate object for the speech synthesizer.

