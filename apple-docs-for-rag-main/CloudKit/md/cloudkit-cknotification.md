

- CloudKit
-  CKNotification 

Class

# CKNotification

The abstract base class for CloudKit notifications.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKNotification
```

## Overview

Use subclasses of `CKNotification` to extract data from push notifications that the system receives, or to fetch a container’s previous push notifications. In both cases, the object indicates the changed data.

`CKNotification` is an abstract class. When you create a notification from a payload dictionary, the init(fromRemoteNotificationDictionary:) method returns an instance of the appropriate subclass. Similarly, when you fetch notifications from a container, you receive instances of a concrete subclass. `CKNotification` provides information about the push notification and its method of delivery. Subclasses contain specific data that provides the changes.

## Topics

### Creating a Notification

convenience init?(fromRemoteNotificationDictionary: [AnyHashable : Any])

Creates a new notification using the specified payload data.

### Identifying the Notification

var notificationID: CKNotification.ID?

The notification’s ID.

class ID

An object that uniquely identifies a push notification that a container sends.

var notificationType: CKNotification.NotificationType

The type of event that generates the notification.

enum NotificationType

Constants that indicate the type of event that generates the push notification.

var containerIdentifier: String?

The ID of the container with the content that triggers the notification.

### Getting the Notification’s Status

var isPruned: Bool

A Boolean value that indicates whether the system removes some push notification content before delivery.

### Accessing the Notification Info

var alertBody: String?

The notification’s alert body.

Deprecated

var alertLocalizationKey: String?

The key that identifies the localized text for the alert body.

Deprecated

var alertLocalizationArgs: [String]?

The fields for building a notification’s alert.

Deprecated

var alertActionLocalizationKey: String?

The key that identifies the localized string for the notification’s action.

Deprecated

var alertLaunchImage: String?

The filename of an image to use as a launch image.

Deprecated

var soundName: String?

The name of the sound file to play when a notification arrives.

Deprecated

var badge: NSNumber?

The value that the app icon’s badge displays.

Deprecated

var category: String?

The name of the action group that corresponds to this notification.

Deprecated

var subscriptionID: CKSubscription.ID?

The ID of the subscription that triggers the notification.

var subscriptionOwnerUserRecordID: CKRecord.ID?

The ID of the user record that creates the subscription that generates the push notification.

var title: String?

The notification’s title.

Deprecated

var titleLocalizationKey: String?

The key that identifies the localized string for the notification’s title.

Deprecated

var titleLocalizationArgs: [String]?

The fields for building a notification’s title.

Deprecated

var subtitle: String?

The notification’s subtitle.

Deprecated

var subtitleLocalizationKey: String?

The key that identifies the localized string for the notification’s subtitle.

Deprecated

var subtitleLocalizationArgs: [String]?

The fields for building a notification’s subtitle.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- CKDatabaseNotification
- CKQueryNotification
- CKRecordZoneNotification

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Base Objects

class CKSubscription

An abstract base class for subscriptions.

class CKDatabaseOperation

The abstract base class for operations that act upon databases in CloudKit.

