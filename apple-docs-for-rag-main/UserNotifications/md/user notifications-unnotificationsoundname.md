

- User Notifications
-  UNNotificationSoundName 

Structure

# UNNotificationSoundName

A string providing the name of a sound file.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
struct UNNotificationSoundName
```

## Topics

### Initializers

init(String)

Creates a notification sound name using the string parameter.

init(rawValue: String)

Creates a notification sound name using the string parameter.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Notification content

Implementing communication notifications

Configure and display your app’s communication notifications by using intents.

protocol UNNotificationContentProviding

A protocol the system uses to provide context relevant to user notifications.

class UNNotificationActionIcon

An icon associated with an action.

class UNMutableNotificationContent

The editable content for a notification.

class UNNotificationContent

The uneditable content of a notification.

class UNNotificationAttachment

A media file associated with a notification.

class UNNotificationSound

The sound played upon delivery of a notification.

