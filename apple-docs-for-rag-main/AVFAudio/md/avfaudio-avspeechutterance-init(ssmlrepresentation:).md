

- AVFAudio
- AVSpeechUtterance
-  init(ssmlRepresentation:) 

Initializer

# init(ssmlRepresentation:)

Creates a speech utterance with an Speech Synthesis Markup Language (SSML) string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init?(ssmlRepresentation string: String)
```

## Parameters 

`string`  

A string to speak that contains valid SSML markup. The initializer returns `nil` if you pass an invalid SSML string.

## Discussion

If using SSML to request voices that fall under certain attributes, the system may split a single utterance into multiple parts and send each to an appropriate synthesizer.

If no voice matches the properties, the utterance uses the voice set in its voice property. If you don’t specify a voice, the system uses its default voice.

Note

Speech utterance properties that affect the prosody of a voice, such as its rate and pitchMultiplier, don’t apply to an utterance that uses an SSML representation.

## See Also

### Creating an utterance

init(string: String)

Creates an utterance with the text string that you specify for the speech synthesizer to speak.

init(attributedString: NSAttributedString)

Creates an utterance with the attributed text string that you specify for the speech synthesizer to speak.

let AVSpeechSynthesisIPANotationAttribute: String

A string that contains International Phonetic Alphabet (IPA) symbols the speech synthesizer uses to control pronunciation of certain words or phrases.

