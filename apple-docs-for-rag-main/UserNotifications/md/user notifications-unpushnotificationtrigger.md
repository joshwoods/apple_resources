

- User Notifications
-  UNPushNotificationTrigger 

Class

# UNPushNotificationTrigger

A trigger condition that indicates Apple Push Notification Service (APNs) has sent the notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UNPushNotificationTrigger
```

## Overview

You don’t create instances of this class yourself. The system creates UNPushNotificationTrigger objects and associates them with requests that originated from Apple Push Notification service. You encounter instances of this class when managing your app’s delivered notification requests, which store an object of this type in their trigger property.

## Relationships

### Inherits From

- UNNotificationTrigger

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

### Triggers

class UNCalendarNotificationTrigger

A trigger condition that causes a notification the system delivers at a specific date and time.

class UNTimeIntervalNotificationTrigger

A trigger condition that causes the system to deliver a notification after the amount of time you specify elapses.

class UNLocationNotificationTrigger

A trigger condition that causes the system to deliver a notification when the user’s device enters or exits a geographic region you specify.

class UNNotificationTrigger

The common behavior for subclasses that trigger the delivery of a local or remote notification.

