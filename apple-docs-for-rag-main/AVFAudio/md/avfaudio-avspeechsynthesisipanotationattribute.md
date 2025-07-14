

- AVFAudio
-  AVSpeechSynthesisIPANotationAttribute 

Global Variable

# AVSpeechSynthesisIPANotationAttribute

A string that contains International Phonetic Alphabet (IPA) symbols the speech synthesizer uses to control pronunciation of certain words or phrases.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
let AVSpeechSynthesisIPANotationAttribute: String
```

## Discussion

For example, the speech synthesizer uses an `AVSpeechSynthesisIPANotationAttribute` instance to control pronunciation of a proper name.

## See Also

### Creating an utterance

init(string: String)

Creates an utterance with the text string that you specify for the speech synthesizer to speak.

init(attributedString: NSAttributedString)

Creates an utterance with the attributed text string that you specify for the speech synthesizer to speak.

init?(ssmlRepresentation: String)

Creates a speech utterance with an Speech Synthesis Markup Language (SSML) string.

