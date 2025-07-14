

- AppKit
- NSSpeechSynthesizer
-  init(voice:) Deprecated

Initializer

# init(voice:)

Initializes the receiver with a voice.

macOS 10.3–14.0Deprecated

``` source
init?(voice: NSSpeechSynthesizer.VoiceName?)
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Parameters 

`voice`  

Identifier of the voice to set as the current voice. When `nil`, the default voice is used. Passing in a specific voice means the initial speaking rate is determined by the synthesizer’s default speaking rate; passing `nil` means the speaking rate is automatically set to the rate the user specifies in Speech preferences.

## Return Value

Initialized speech synthesizer or `nil` when the voice identified by `voiceIdentifier` is not available or when there’s an allocation error.

## See Also

### Related Documentation

Speech Programming Topics

class var availableVoices: [NSSpeechSynthesizer.VoiceName]

Provides the identifiers of the voices available on the system.

Deprecated

