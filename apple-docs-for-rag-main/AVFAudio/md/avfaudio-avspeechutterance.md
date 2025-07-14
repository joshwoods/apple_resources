

- AVFAudio
-  AVSpeechUtterance 

Class

# AVSpeechUtterance

An object that encapsulates the text for speech synthesis and parameters that affect the speech.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class AVSpeechUtterance
```

## Overview

An `AVSpeechUtterance` is the basic unit of speech synthesis.

To synthesize speech, create an `AVSpeechUtterance` instance with text you want a speech synthesizer to speak. Optionally, change the voice, pitchMultiplier, volume, rate, preUtteranceDelay, or postUtteranceDelay parameters for the utterance. Pass the utterance to an instance of AVSpeechSynthesizer to begin speech, or enqueue the utterance to speak later if the synthesizer is already speaking.

Split a body of text into multiple utterances if you want to apply different speech parameters. For example, you can emphasize a sentence by increasing the pitch and decreasing the rate of that utterance relative to others, or you can introduce pauses between sentences by putting each into an utterance with a leading or trailing delay.

Set and use the AVSpeechSynthesizerDelegate to receive notifications when the synthesizer starts or finishes speaking an utterance. Create an utterance for each meaningful unit in a body of text if you want to receive notifications as its speech progresses.

## Topics

### Creating an utterance

init(string: String)

Creates an utterance with the text string that you specify for the speech synthesizer to speak.

init(attributedString: NSAttributedString)

Creates an utterance with the attributed text string that you specify for the speech synthesizer to speak.

let AVSpeechSynthesisIPANotationAttribute: String

A string that contains International Phonetic Alphabet (IPA) symbols the speech synthesizer uses to control pronunciation of certain words or phrases.

init?(ssmlRepresentation: String)

Creates a speech utterance with an Speech Synthesis Markup Language (SSML) string.

### Configuring an utterance

var voice: AVSpeechSynthesisVoice?

The voice the speech synthesizer uses when speaking the utterance.

var pitchMultiplier: Float

The baseline pitch the speech synthesizer uses when speaking the utterance.

var volume: Float

The volume the speech synthesizer uses when speaking the utterance.

var prefersAssistiveTechnologySettings: Bool

A Boolean that specifies whether assistive technology settings take precedence over the property values of this utterance.

### Configuring utterance timing

var rate: Float

The rate the speech synthesizer uses when speaking the utterance.

let AVSpeechUtteranceMinimumSpeechRate: Float

The minimum rate the speech synthesizer uses when speaking an utterance.

let AVSpeechUtteranceMaximumSpeechRate: Float

The maximum rate the speech synthesizer uses when speaking an utterance.

let AVSpeechUtteranceDefaultSpeechRate: Float

The default rate the speech synthesizer uses when speaking an utterance.

var preUtteranceDelay: TimeInterval

The amount of time the speech synthesizer pauses before speaking the utterance.

var postUtteranceDelay: TimeInterval

The amount of time the speech synthesizer pauses after speaking an utterance before handling the next utterance in the queue.

### Inspecting utterance text

var speechString: String

A string that contains the text for speech synthesis.

var attributedSpeechString: NSAttributedString

An attributed string that contains the text for speech synthesis.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Spoken text attributes

class AVSpeechSynthesisVoice

A distinct voice for use in speech synthesis.

