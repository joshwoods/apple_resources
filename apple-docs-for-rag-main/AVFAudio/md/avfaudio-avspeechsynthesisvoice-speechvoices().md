

- AVFAudio
- AVSpeechSynthesisVoice
-  speechVoices() 

Type Method

# speechVoices()

Retrieves all available voices on the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func speechVoices() -> [AVSpeechSynthesisVoice]
```

## Return Value

An array of voices.

## Discussion

Use the language property to identify each voice by its language and locale.

## See Also

### Obtaining voices

init?(identifier: String)

Retrieves a voice for the identifier you specify.

init?(language: String?)

Retrieves a voice for the BCP 47 code language code you specify.

let AVSpeechSynthesisVoiceIdentifierAlex: String

The voice that the system identifies as Alex.

