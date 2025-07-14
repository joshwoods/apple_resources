

- CloudKit
-  CKDatabaseNotification 

Class

# CKDatabaseNotification

A notification that triggers when the contents of a database change.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class CKDatabaseNotification
```

## Overview

Database subscriptions execute when changes happen in any of a database’s record zones, for example, when CloudKit saves a new record. When the subscription registers a change, it sends push notifications to the user’s devices to inform your app about the change. You can then fetch the changes and cache them on-device. When appropriate, CloudKit excludes the device where the change originates.

You configure a subscription’s notifications by setting it’s notificationInfo property. Do this before you save it to the server. A subscription generates either high-priority or medium-priority push notifications. CloudKit delivers medium-priority notifications to your app in the background. High-priority notifications are visual and the system displays them to the user. Visual notifications need the user’s permission. For more information, see Asking permission to use notifications.

A subscription uses CKSubscription.NotificationInfo to configure its notifications. For background delivery, set only its shouldSendContentAvailable property to true. If you set any other property, CloudKit treats the notification as high-priority.

Note

To receive silent push notifications, add the Background Modes capability to your Xcode project and select the “Background fetch” and “Remote notifications” options.

Don’t rely on push notifications for specific changes because the system can coalesce them. CloudKit can omit data to keep the notification’s payload size under the APNs size limit. Consider notifications an indication of remote changes. Use databaseScope to determine which database has changes, and then CKFetchDatabaseChangesOperation to fetch those changes. A notification’s isPruned property is true if CloudKit omits data.

You don’t instantiate this class. Instead, implement application(_:didReceiveRemoteNotification:fetchCompletionHandler:) in your app delegate. Initialize CKNotification with the `userInfo` dictionary that CloudKit passes to the method. This returns an instance of the appropriate subclass. Use the notificationType property to determine the type. Then cast to that type to access type-specific properties and methods.

## Topics

### Getting the Database Scope

var databaseScope: CKDatabase.Scope

The type of database.

## Relationships

### Inherits From

- CKNotification

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Database Changes

class CKDatabaseSubscription

A subscription that generates push notifications when CloudKit modifies records in a database.

class CKFetchDatabaseChangesOperation

An operation that fetches database changes.

