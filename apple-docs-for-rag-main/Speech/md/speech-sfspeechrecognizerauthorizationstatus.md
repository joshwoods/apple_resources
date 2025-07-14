

- Speech
-  SFSpeechRecognizerAuthorizationStatus 

Enumeration

# SFSpeechRecognizerAuthorizationStatus

The app’s authorization to perform speech recognition.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
enum SFSpeechRecognizerAuthorizationStatus
```

## Topics

### Authorization Statuses

case notDetermined

The app’s authorization status has not yet been determined.

case denied

The user denied your app’s request to perform speech recognition.

case restricted

The device prevents your app from performing speech recognition.

case authorized

The user granted your app’s request to perform speech recognition.

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

### Requesting Authorization from the User

class func requestAuthorization((SFSpeechRecognizerAuthorizationStatus) -> Void)

Asks the user to allow your app to perform speech recognition.

class func authorizationStatus() -> SFSpeechRecognizerAuthorizationStatus

Returns your app’s current authorization to perform speech recognition.

