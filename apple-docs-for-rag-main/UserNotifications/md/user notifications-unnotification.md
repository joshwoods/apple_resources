

- User Notifications
-  UNNotification 

Class

# UNNotification

The data for a local or remote notification the system delivers to your app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UNNotification
```

## Overview

A UNNotification object contains the initial notification request, which contains the notification’s payload, and the date that the system delivered the notification.

Don’t create notification objects directly. When handling notifications, the system delivers notification objects to your UNUserNotificationCenterDelegate object. The UNUserNotificationCenter object also maintains the list of notifications that the system delivers, and you use the getDeliveredNotifications(completionHandler:) method to retrieve those objects.

## Topics

### Getting the Notification Details

var request: UNNotificationRequest

The notification request containing the payload and trigger condition for the notification.

var date: Date

The delivery date of the notification.

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

### Notification requests

Scheduling a notification locally from your app

Create and schedule notifications from your app when you want to get the user’s attention.

class UNNotificationRequest

A request to schedule a local notification, which includes the content of the notification and the trigger conditions for delivery.

