

- AppKit
- NSSpeechSynthesizer
-  NSSpeechSynthesizer.VoiceName Deprecated

Structure

# NSSpeechSynthesizer.VoiceName

macOS 10.3–14.0Deprecated

``` source
struct VoiceName
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Topics

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Speech Synthesizer Information

class var availableVoices: [NSSpeechSynthesizer.VoiceName]

Provides the identifiers of the voices available on the system.

Deprecated

class func attributes(forVoice: NSSpeechSynthesizer.VoiceName) -> [NSSpeechSynthesizer.VoiceAttributeKey : Any]

Provides the attribute dictionary of a voice.

Deprecated

class var defaultVoice: NSSpeechSynthesizer.VoiceName

Provides the identifier of the default voice.

Deprecated

struct VoiceAttributeKey

The following constants are keys for the dictionary returned by attributes(forVoice:).

Deprecated

