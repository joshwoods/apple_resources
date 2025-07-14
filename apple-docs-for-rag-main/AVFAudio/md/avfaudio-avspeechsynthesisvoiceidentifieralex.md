

- AVFAudio
-  AVSpeechSynthesisVoiceIdentifierAlex 

Global Variable

# AVSpeechSynthesisVoiceIdentifierAlex

The voice that the system identifies as Alex.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.14+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let AVSpeechSynthesisVoiceIdentifierAlex: String
```

## Discussion

The Alex voice is only available for the `en-US` language code.

## See Also

### Obtaining voices

init?(identifier: String)

Retrieves a voice for the identifier you specify.

init?(language: String?)

Retrieves a voice for the BCP 47 code language code you specify.

class func speechVoices() -> [AVSpeechSynthesisVoice]

Retrieves all available voices on the device.

