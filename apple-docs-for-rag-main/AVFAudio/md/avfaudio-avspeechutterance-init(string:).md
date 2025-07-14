

- AVFAudio
- AVSpeechUtterance
-  init(string:) 

Initializer

# init(string:)

Creates an utterance with the text string that you specify for the speech synthesizer to speak.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(string: String)
```

## Parameters 

`string`  

A string that contains the text to speak.

## Return Value

An AVSpeechUtterance object that can speak the specified text.

## Discussion

To speak the text, pass the utterance to an instance of AVSpeechSynthesizer.

## See Also

### Creating an utterance

init(attributedString: NSAttributedString)

Creates an utterance with the attributed text string that you specify for the speech synthesizer to speak.

let AVSpeechSynthesisIPANotationAttribute: String

A string that contains International Phonetic Alphabet (IPA) symbols the speech synthesizer uses to control pronunciation of certain words or phrases.

init?(ssmlRepresentation: String)

Creates a speech utterance with an Speech Synthesis Markup Language (SSML) string.

