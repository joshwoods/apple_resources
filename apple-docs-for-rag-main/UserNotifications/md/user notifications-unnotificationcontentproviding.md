

- User Notifications
-  UNNotificationContentProviding 

Protocol

# UNNotificationContentProviding

A protocol the system uses to provide context relevant to user notifications.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol UNNotificationContentProviding : NSObjectProtocol
```

## Overview

The system allows only objects in the Apple SDK that conform to `UNNotificationContentProviding`. The system ignores objects outside of the Apple SDK that your app conforms to `UNNotificationContentProviding`.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UNNotificationAttributedMessageContext

## See Also

### Notification content

Implementing communication notifications

Configure and display your app’s communication notifications by using intents.

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

struct UNNotificationSoundName

A string providing the name of a sound file.

