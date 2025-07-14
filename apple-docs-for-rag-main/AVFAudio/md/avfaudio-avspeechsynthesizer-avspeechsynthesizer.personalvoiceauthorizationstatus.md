

- AVFAudio
- AVSpeechSynthesizer
-  AVSpeechSynthesizer.PersonalVoiceAuthorizationStatus 

Enumeration

# AVSpeechSynthesizer.PersonalVoiceAuthorizationStatus

An enumeration that models the personal voices authorization status.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum PersonalVoiceAuthorizationStatus
```

## Topics

### Authorization statuses

case authorized

The user granted your app’s request to use personal voices.

case denied

The user denied your app’s request to use personal voices.

case notDetermined

The app hasn’t requested authorization to use personal voices.

case unsupported

The device doesn’t support personal voices.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enabling personal voices

class var personalVoiceAuthorizationStatus: AVSpeechSynthesizer.PersonalVoiceAuthorizationStatus

Your app’s authorization to use personal voices.

class let availableVoicesDidChangeNotification: NSNotification.Name

A notification that indicates a change in available voices for speech synthesis.

class func requestPersonalVoiceAuthorization(completionHandler: (AVSpeechSynthesizer.PersonalVoiceAuthorizationStatus) -> Void)

Prompts the user to authorize your app to use personal voices.

