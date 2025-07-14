

- CloudKit
- CKNotification
-  CKNotification.ID 

Class

# CKNotification.ID

An object that uniquely identifies a push notification that a container sends.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class ID
```

## Overview

You don’t create notification IDs directly. The server creates them when it creates instances of CKNotification that correspond to the push notifications that CloudKit sends to your app. You can compare two IDs using the isEqual(_:) method to determine whether two notifications are the same. This class defines no methods or properties.

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
- Sendable

## See Also

### Identifying the Notification

var notificationID: CKNotification.ID?

The notification’s ID.

var notificationType: CKNotification.NotificationType

The type of event that generates the notification.

enum NotificationType

Constants that indicate the type of event that generates the push notification.

var containerIdentifier: String?

The ID of the container with the content that triggers the notification.

