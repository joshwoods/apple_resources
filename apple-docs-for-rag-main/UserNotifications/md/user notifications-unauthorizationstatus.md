

- User Notifications
-  UNAuthorizationStatus 

Enumeration

# UNAuthorizationStatus

Constants indicating whether the app is allowed to schedule notifications.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum UNAuthorizationStatus
```

## Topics

### Status

case notDetermined

The user hasn’t yet made a choice about whether the app is allowed to schedule notifications.

case denied

The app isn’t authorized to schedule or receive notifications.

case authorized

The app is authorized to schedule or receive notifications.

case provisional

The application is provisionally authorized to post noninterruptive user notifications.

case ephemeral

The app is authorized to schedule or receive notifications for a limited amount of time.

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

### Getting the Authorization Status

var authorizationStatus: UNAuthorizationStatus

The app’s ability to schedule and receive local and remote notifications.

