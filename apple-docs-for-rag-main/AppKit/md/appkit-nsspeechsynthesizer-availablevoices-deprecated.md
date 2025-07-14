

- AppKit
- NSSpeechSynthesizer
-  availableVoices Deprecated

Type Property

# availableVoices

Provides the identifiers of the voices available on the system.

macOS 10.3–14.0Deprecated

``` source
class var availableVoices: [NSSpeechSynthesizer.VoiceName] { get }
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Return Value

Array of strings representing the identifiers of each voice available on the system.

## See Also

### Related Documentation

func setVoice(NSSpeechSynthesizer.VoiceName?) -> Bool

Sets the receiver’s current voice.

Deprecated

### Getting Speech Synthesizer Information

class func attributes(forVoice: NSSpeechSynthesizer.VoiceName) -> [NSSpeechSynthesizer.VoiceAttributeKey : Any]

Provides the attribute dictionary of a voice.

Deprecated

class var defaultVoice: NSSpeechSynthesizer.VoiceName

Provides the identifier of the default voice.

Deprecated

struct VoiceNameDeprecated

struct VoiceAttributeKey

The following constants are keys for the dictionary returned by attributes(forVoice:).

Deprecated

