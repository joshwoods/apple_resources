

- AVFAudio
- AVSpeechSynthesisVoice
-  init(identifier:) 

Initializer

# init(identifier:)

Retrieves a voice for the identifier you specify.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.14+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(identifier: String)
```

## Parameters 

`identifier`  

The unique identifier for a voice.

## Return Value

A voice for the specified identifier if the identifier is valid and the voice is available on the device; otherwise, `nil`.

## See Also

### Obtaining voices

init?(language: String?)

Retrieves a voice for the BCP 47 code language code you specify.

class func speechVoices() -> [AVSpeechSynthesisVoice]

Retrieves all available voices on the device.

let AVSpeechSynthesisVoiceIdentifierAlex: String

The voice that the system identifies as Alex.

