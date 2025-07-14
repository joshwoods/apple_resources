

- User Notifications
-  UNNotificationInterruptionLevel 

Enumeration

# UNNotificationInterruptionLevel

Constants that indicate the importance and delivery timing of a notification.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum UNNotificationInterruptionLevel
```

## Mentioned in 

Generating a remote notification

## Topics

### Enumeration Cases

case active

The system presents the notification immediately, lights up the screen, and can play a sound.

case critical

The system presents the notification immediately, lights up the screen, and bypasses the mute switch to play a sound.

case passive

The system adds the notification to the notification list without lighting up the screen or playing a sound.

case timeSensitive

The system presents the notification immediately, lights up the screen, can play a sound, and breaks through system notification controls.

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

### Integrating with the system

var sound: UNNotificationSound?

The sound that plays when the system delivers the notification.

var interruptionLevel: UNNotificationInterruptionLevel

The notification’s importance and required delivery timing.

var relevanceScore: Double

The score the system uses to determine if the notification is the summary’s featured notification.

var filterCriteria: String?

The criteria the system evaluates to determine if it displays the notification in the current Focus.

