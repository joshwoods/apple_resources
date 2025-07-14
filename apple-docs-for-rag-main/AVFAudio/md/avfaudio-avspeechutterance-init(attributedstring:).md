

- AVFAudio
- AVSpeechUtterance
-  init(attributedString:) 

Initializer

# init(attributedString:)

Creates an utterance with the attributed text string that you specify for the speech synthesizer to speak.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(attributedString string: NSAttributedString)
```

## Parameters 

`string`  

A string that contains the text to speak.

## Discussion

To speak the text, pass the utterance to an instance of AVSpeechSynthesizer.

## See Also

### Creating an utterance

init(string: String)

Creates an utterance with the text string that you specify for the speech synthesizer to speak.

let AVSpeechSynthesisIPANotationAttribute: String

A string that contains International Phonetic Alphabet (IPA) symbols the speech synthesizer uses to control pronunciation of certain words or phrases.

init?(ssmlRepresentation: String)

Creates a speech utterance with an Speech Synthesis Markup Language (SSML) string.

