

- CloudKit
- CKSubscription
-  CKSubscription.NotificationInfo 

Class

# CKSubscription.NotificationInfo

An object that describes the configuration of a subscription’s push notifications.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 6.0+

``` source
class NotificationInfo
```

## Overview

When configuring a subscription, use this class to specify the type of push notifications you want to generate when conditions meet the subscription’s trigger. You can provide content that the system displays to the user, describe the sounds to play, and indicate whether the app’s icon has a badge. You can request that the notification include information about the record that triggers it.

When your app receives a push notification that a subscription generates, instantiate an instance of CKNotification using the init(fromRemoteNotificationDictionary:) method and pass the notification’s payload. The object that the method returns contains the data you specify when configuring the subscription.

For more information about push notification alerts and how they display to the user, see Apple Push Notification Service in Local and Remote Notification Programming Guide.

Note

If you don’t set any of the alertBody, soundName, or shouldBadge properties, CloudKit sends the push notification using a lower priority and doesn’t display any content to the user.

## Topics

### Creating Notification Information

convenience init(alertBody: String?, alertLocalizationKey: String?, alertLocalizationArgs: [CKRecord.FieldKey], title: String?, titleLocalizationKey: String?, titleLocalizationArgs: [CKRecord.FieldKey], subtitle: String?, subtitleLocalizationKey: String?, subtitleLocalizationArgs: [CKRecord.FieldKey], alertActionLocalizationKey: String?, alertLaunchImage: String?, soundName: String?, desiredKeys: [CKRecord.FieldKey], shouldBadge: Bool, shouldSendContentAvailable: Bool, shouldSendMutableContent: Bool, category: String?, collapseIDKey: String?)

Creates a notification with the specified values.

### Grouping Notifications

var category: String?

The name of the action group that corresponds to this notification.

var collapseIDKey: String?

A value that the system uses to coalesce unseen push notifications.

### Displaying Badges

var shouldBadge: Bool

A Boolean value that determines whether an app’s icon badge increments its value.

### Accessing the Notification Alert

var alertBody: String?

The text for the notification’s alert.

var alertLocalizationKey: String?

The key that identifies the localized string for the notification’s alert.

var alertLocalizationArgs: [CKRecord.FieldKey]?

The fields for building a notification’s alert.

var alertActionLocalizationKey: String?

The key that identifies the localized string for the notification’s action.

var alertLaunchImage: String?

The filename of an image to use as a launch image.

var soundName: String?

The filename of the sound file to play when a notification arrives.

### Accessing the Notification Info

var shouldSendContentAvailable: Bool

A Boolean value that indicates whether the push notification includes the content available flag.

var shouldSendMutableContent: Bool

A Boolean value that indicates whether the push notification sets the mutable content flag.

### Accessing the Record’s Data

var desiredKeys: [CKRecord.FieldKey]?

The names of fields to include in the push notification’s payload.

### Accessing the Notification Title

var title: String?

The notification’s title.

var titleLocalizationKey: String?

The key that identifies the localized string for the notification’s title.

var titleLocalizationArgs: [CKRecord.FieldKey]?

The fields for building a notification’s title.

### Accessing the Notification Subtitle

var subtitle: String?

The notification’s subtitle.

var subtitleLocalizationKey: String?

The key that identifies the localized string for the notification’s subtitle.

var subtitleLocalizationArgs: [CKRecord.FieldKey]?

The fields for building a notification’s subtitle.

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

### Specifying the Push Notification Data

var notificationInfo: CKSubscription.NotificationInfo?

The configuration for a subscription’s push notifications.

