

- User Notifications
-  UNNotificationActionIcon 

Class

# UNNotificationActionIcon

An icon associated with an action.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class UNNotificationActionIcon
```

## Topics

### Essentials

convenience init(systemImageName: String)

Creates an action icon by using a system symbol image.

convenience init(templateImageName: String)

Creates an action icon based on an image in your app’s bundle, preferably in an asset catalog.

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

## See Also

### Notification content

Implementing communication notifications

Configure and display your app’s communication notifications by using intents.

protocol UNNotificationContentProviding

A protocol the system uses to provide context relevant to user notifications.

class UNMutableNotificationContent

The editable content for a notification.

class UNNotificationContent

The uneditable content of a notification.

class UNNotificationAttachment

A media file associated with a notification.

class UNNotificationSound

The sound played upon delivery of a notification.

struct UNNotificationSoundName

A string providing the name of a sound file.

