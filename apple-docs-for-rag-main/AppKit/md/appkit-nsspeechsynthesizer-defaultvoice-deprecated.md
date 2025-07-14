

- AppKit
- NSSpeechSynthesizer
-  defaultVoice Deprecated

Type Property

# defaultVoice

Provides the identifier of the default voice.

macOS 10.3–14.0Deprecated

``` source
class var defaultVoice: NSSpeechSynthesizer.VoiceName { get }
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Return Value

Identifier of the default voice.

## See Also

### Getting Speech Synthesizer Information

class var availableVoices: [NSSpeechSynthesizer.VoiceName]

Provides the identifiers of the voices available on the system.

Deprecated

class func attributes(forVoice: NSSpeechSynthesizer.VoiceName) -> [NSSpeechSynthesizer.VoiceAttributeKey : Any]

Provides the attribute dictionary of a voice.

Deprecated

struct VoiceNameDeprecated

struct VoiceAttributeKey

The following constants are keys for the dictionary returned by attributes(forVoice:).

Deprecated

