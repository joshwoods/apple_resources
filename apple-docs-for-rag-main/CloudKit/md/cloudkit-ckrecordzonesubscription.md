

- CloudKit
-  CKRecordZoneSubscription 

Class

# CKRecordZoneSubscription

A subscription that generates push notifications when CloudKit modifies records in a specific record zone.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 6.0+

``` source
class CKRecordZoneSubscription
```

## Overview

Subscriptions track the creation, modification, and deletion of records in a database, and are fundamental in keeping data on the user’s device up to date. A subscription applies only to the user that creates it. When a subscription registers a change, such as CloudKit saving a new record, it sends push notifications to the user’s devices to inform your app about the change. You can then fetch the changes and cache them on-device. When appropriate, the server excludes the device where the change originates.

Note

You don’t need to explicitly enable push notifications for your App ID to receive subscription notifications. Xcode automatically adds the entitlement when you enable the CloudKit capability. For more information, see Enabling CloudKit in Your App. To use silent push notifications, add the Background Modes capability in your Xcode project and then select the “Background fetch” and “Remote notifications” options.

Record zone subscriptions execute whenever a change happens in the record zone you specify when you create the subscription. You can further specialize the subscription by setting its recordType property to a specific record type. This limits the scope of the subscription to only track changes to records of that type and reduces the number of notifications it generates.

Note

Only the private database supports record zone subscriptions. If you attempt to save a record zone subscription in a public or shared database, CloudKit returns an error.

Create any subscriptions on your app’s first launch. After you initialize a subscription, save it to the server using CKModifySubscriptionsOperation. When the operation completes, record that state on-device (in UserDefaults, for example). You can then check that state on subsequent launches to prevent unnecessary trips to the server.

To configure the notification that the subscription generates, set the subscription’s notificationInfo property. Because the system coalesces notifications, don’t rely on them for specific changes. CloudKit can omit data to keep the payload size under the APNs size limit. Consider notifications an indication of remote changes and use CKFetchRecordZoneChangesOperation to fetch the changed records. Server change tokens allow you to limit the fetch results to just the changes since your previous fetch.

The example below shows how to create a record zone subscription in the user’s private database, configure the notifications it generates — in this case, silent push notifications — and then save that subscription to the server:

```
// Only proceed if the subscription doesn't already exist.
if([[NSUserDefaults standardUserDefaults]
    boolForKey:@"didCreateFeedSubscription"] == NO) {

    // Create a subscription that's scoped to a specific record zone. Provide
    // a subscription ID that's unique within the context of the user's 
    // private database.
    CKRecordZoneSubscription *subscription =
    [[CKRecordZoneSubscription alloc]
     initWithZoneID:recordZone.zoneID
     subscriptionID:@"feed-changes"];

    // Scope the subscription to just the 'FeedItem' record type.
    subscription.recordType = @"FeedItem";

    // Configure the notification so that the system delivers it silently
    // and therefore doesn't require permission from the user.
    CKNotificationInfo *notificationInfo = [CKNotificationInfo new];
    notificationInfo.shouldSendContentAvailable = YES;
    subscription.notificationInfo = notificationInfo;

    // Create an operation that saves the subscription to the server.
    CKModifySubscriptionsOperation *operation = 
        [[CKModifySubscriptionsOperation alloc]
         initWithSubscriptionsToSave:@[subscription]
         subscriptionIDsToDelete:NULL];

    operation.modifySubscriptionsCompletionBlock = 
        ^(NSArray *subscriptions, NSArray *deleted, NSError *error) {
        if (error) {
            // Handle the error.
        } else {
            // Record that the system successfully creates the subscription
            // to prevent unnecessary trips to the server in later launches.
            [[NSUserDefaults standardUserDefaults] 
             setBool:YES forKey:@"didCreateFeedSubscription"];
        }
    };

    // Set an appropriate QoS and add the operation to the private
    // database's operation queue to execute it.
    operation.qualityOfService = NSQualityOfServiceUtility;
    [CKContainer.defaultContainer.privateCloudDatabase addOperation:operation];
}
```

## Topics

### Creating a Zone-Based Subscription

convenience init(zoneID: CKRecordZone.ID)

Creates a subscription for all records in the specified record zone.

Deprecated

convenience init(zoneID: CKRecordZone.ID, subscriptionID: CKSubscription.ID)

Creates a named subscription for all records in the specified record zone.

init(coder: NSCoder)

Creates a zone-based subscription from a serialized instance.

### Accessing the Subscription Metadata

var recordType: CKRecord.RecordType?

The type of record that the subscription queries.

var zoneID: CKRecordZone.ID

The ID of the record zone that the subscription queries.

## Relationships

### Inherits From

- CKSubscription

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

### Record Zone Changes

class CKRecordZoneNotification

A notification that triggers when the contents of a record zone change.

class CKFetchRecordZoneChangesOperation

An operation that fetches record zone changes.

