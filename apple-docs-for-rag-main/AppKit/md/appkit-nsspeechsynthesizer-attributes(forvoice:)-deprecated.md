

- AppKit
- NSSpeechSynthesizer
-  attributes(forVoice:) Deprecated

Type Method

# attributes(forVoice:)

Provides the attribute dictionary of a voice.

macOS 10.3–14.0Deprecated

``` source
class func attributes(forVoice voice: NSSpeechSynthesizer.VoiceName) -> [NSSpeechSynthesizer.VoiceAttributeKey : Any]
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Parameters 

`voice`  

Identifier of the voice whose attributes you want to obtain.

## Return Value

Attribute dictionary of the voice identified by `voiceIdentifier`. The attributes keys and value types are listed in `Voice Attributes Keys`

## See Also

### Getting Speech Synthesizer Information

class var availableVoices: [NSSpeechSynthesizer.VoiceName]

Provides the identifiers of the voices available on the system.

Deprecated

class var defaultVoice: NSSpeechSynthesizer.VoiceName

Provides the identifier of the default voice.

Deprecated

struct VoiceNameDeprecated

struct VoiceAttributeKey

The following constants are keys for the dictionary returned by attributes(forVoice:).

Deprecated

