

- User Notifications
-  UNNotificationTrigger 

Class

# UNNotificationTrigger

The common behavior for subclasses that trigger the delivery of a local or remote notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UNNotificationTrigger
```

## Overview

The UNNotificationTrigger class is an abstract class for representing an event that triggers the delivery of a notification. You don’t create instances of this class directly. Instead, you instantiate the concrete subclass that defines the trigger condition you want for your notification. You then assign the resulting object to the UNNotificationRequest object that you use to schedule your notification.

Concrete trigger classes include the following:

- UNTimeIntervalNotificationTrigger

- UNCalendarNotificationTrigger

- UNLocationNotificationTrigger

- UNPushNotificationTrigger

## Topics

### Configuring the Trigger’s Behavior

var repeats: Bool

A Boolean value indicating whether the system reschedules the notification after it’s delivered.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UNCalendarNotificationTrigger
- UNLocationNotificationTrigger
- UNPushNotificationTrigger
- UNTimeIntervalNotificationTrigger

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

class UNPushNotificationTrigger

A trigger condition that indicates Apple Push Notification Service (APNs) has sent the notification.

