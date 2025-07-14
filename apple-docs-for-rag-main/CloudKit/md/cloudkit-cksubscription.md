

- CloudKit
-  CKSubscription 

Class

# CKSubscription

An abstract base class for subscriptions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKSubscription
```

## Overview

A subscription acts like a persistent query on the server that can track the creation, deletion, and modification of records. When changes occur, they trigger the delivery of push notifications so that your app can respond appropriately.

Subscriptions don’t become active until you save them to the server and the server has time to index them. To save a subscription, use an instance of CKModifySubscriptionsOperation or the save(_:completionHandler:) method of CKDatabase. To cancel a subscription, delete the corresponding subscription from the server.

Note

You don’t need to enable push notifications for the app’s explicit App ID in your developer account at developer.apple.com to receive subscription notifications. Xcode automatically adds the APNs entitlement to your entitlement file when you enable CloudKit. To learn about enabling CloudKit, see Enabling CloudKit in Your App.

Most of a subscription’s configuration happens at initialization time. You must, however, specify how to deliver push notifications to the user’s device. Use the notificationInfo property to configure the delivery options. You must save the subscription before the changes take effect.

Note

Create subscriptions in the development environment first and then promote them to production. Attempting to create a subscription directly in the production environment results in an error.

### Handling the Resulting Push Notifications

When CloudKit modifies a record and triggers a subscription, the server sends push notifications to all devices with that subscription except for the one that makes the original changes. For subscription-based push notifications, the server can add data to the notification payload that indicates the condition that triggers the notification. In the application(_:didReceiveRemoteNotification:fetchCompletionHandler:) method of your app delegate, create a CKNotification object from the provided `userInfo` dictionary. You can then query it for the information that’s relevant to the notification.

In addition to sending a record ID with a push notification, you can ask the server to send a limited amount of data from the record that triggers the notification. Use the desiredKeys property of the object you assign to notificationInfo to specify the keys to include.

APNs limits the size of a push notification’s payload and CloudKit may omit keys and other pieces of data to keep the payload’s size under that limit. If this happens, you can fetch the entire payload from the server using an instance of `CKFetchNotificationChangesOperation`. This operation provides instances of CKQueryNotification or CKRecordZoneNotification, which contain information about the push notifications that CloudKit delivers to your app.

## Topics

### Specifying the Push Notification Data

var notificationInfo: CKSubscription.NotificationInfo?

The configuration for a subscription’s push notifications.

class NotificationInfo

An object that describes the configuration of a subscription’s push notifications.

### Accessing the Subscription Metadata

var subscriptionID: CKSubscription.ID

The subscription’s unique identifier.

typealias ID

A type that represents a subscription’s identifier.

var subscriptionType: CKSubscription.SubscriptionType

The behavior that a subscription provides.

enum SubscriptionType

Constants that identify a subscription’s behavior.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CKDatabaseSubscription
- CKQuerySubscription
- CKRecordZoneSubscription

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

### Base Objects

class CKNotification

The abstract base class for CloudKit notifications.

class CKDatabaseOperation

The abstract base class for operations that act upon databases in CloudKit.

