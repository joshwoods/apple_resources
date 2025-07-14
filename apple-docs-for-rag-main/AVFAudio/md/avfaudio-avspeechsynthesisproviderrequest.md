

- AVFAudio
-  AVSpeechSynthesisProviderRequest 

Class

# AVSpeechSynthesisProviderRequest

An object that represents the text to synthesize and the voice to use.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class AVSpeechSynthesisProviderRequest
```

## Topics

### Creating a request

init(ssmlRepresentation: String, voice: AVSpeechSynthesisProviderVoice)

Creates a request with a voice and a description.

### Inspecting a request

var ssmlRepresentation: String

The description of the text to synthesize.

var voice: AVSpeechSynthesisProviderVoice

The voice to use in the speech request.

class AVSpeechSynthesisProviderVoice

An object that represents a voice that an audio unit provides to its host.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Rendering speech

func synthesizeSpeechRequest(AVSpeechSynthesisProviderRequest)

Sets the text to synthesize and the voice to use.

