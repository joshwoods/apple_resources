

- AVFAudio
-  AVAudioVoiceProcessingSpeechActivityEvent 

Enumeration

# AVAudioVoiceProcessingSpeechActivityEvent

Types of speech activity events.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
enum AVAudioVoiceProcessingSpeechActivityEvent
```

## Topics

### Events

case started

Indicates the start of speech activity.

case ended

Indicates the end of speech activity.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling Muted Speech Events

func setMutedSpeechActivityEventListener(((AVAudioVoiceProcessingSpeechActivityEvent) -> Void)?) -> Bool

