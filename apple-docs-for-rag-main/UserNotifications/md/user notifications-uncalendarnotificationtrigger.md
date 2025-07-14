

- User Notifications
-  UNCalendarNotificationTrigger 

Class

# UNCalendarNotificationTrigger

A trigger condition that causes a notification the system delivers at a specific date and time.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UNCalendarNotificationTrigger
```

## Overview

Create a UNCalendarNotificationTrigger object when you want to schedule the delivery of a local notification at the date and time you specify. You use an NSDateComponents object to specify only the time values that you want the system to use to determine the matching date and time.

Listing 1 creates a trigger that delivers its notification every morning at 8:30. The repeating behavior is achieved by specifying `true` for the `repeats` parameter when creating the trigger.

Listing 1. Creating a trigger that repeats at a specific time

- Swift
- Objective-C

```
var date = DateComponents()
date.hour = 8
date.minute = 30 
let trigger = UNCalendarNotificationTrigger(dateMatching: date, repeats: true)
```

```
```

## Topics

### Creating a Calendar Trigger

convenience init(dateMatching: DateComponents, repeats: Bool)

Creates a calendar trigger using the date components parameter.

### Getting the Trigger Information

func nextTriggerDate() -> Date?

The next date at which the trigger conditions are met.

var dateComponents: DateComponents

The date components to construct this object.

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

class UNTimeIntervalNotificationTrigger

A trigger condition that causes the system to deliver a notification after the amount of time you specify elapses.

class UNLocationNotificationTrigger

A trigger condition that causes the system to deliver a notification when the user’s device enters or exits a geographic region you specify.

class UNPushNotificationTrigger

A trigger condition that indicates Apple Push Notification Service (APNs) has sent the notification.

class UNNotificationTrigger

The common behavior for subclasses that trigger the delivery of a local or remote notification.

