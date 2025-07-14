

- CloudKit JS
-  CloudKit.Subscription 

Structure

# CloudKit.Subscription

A subscription, which is a persistent query on the server that tracks the creation, deletion, and modification of records.

CloudKit JS 1.0+

``` source
dictionary CloudKit.Subscription {
 String subscriptionType;
 String subscriptionID;
 CloudKit.ZoneID zoneID;
 CloudKit.NotificationInfo notificationInfo;
 Boolean zoneWide;
 String[] firesOn;
 Boolean firesOnce;
 Query query;
};
```

## Overview

The `CloudKit.Subscription` dictionary is the same as the dictionary described in Subscription Dictionary in CloudKit Web Services Reference.

## Topics

### Instance Properties

firesOn

An array of keywords that specify the actions that should trigger push notifications. Possible values in the array are: `"create"`, `"update"`, and `"delete"`. This key is not used if `query` is null.

firesOnce

A Boolean value indicating whether push notifications should be triggered once. If `true`, push notifications are sent once. If `false`, they can be sent multiple times. The default value is `false`.

notificationInfo

A dictionary containing information about how the system should alert the user.

query

The matching criteria to apply to records.

subscriptionID

A unique identifier for the subscription.

subscriptionType

The type of subscription. Possible values are: `"zone"`, and `"query”`. This key is required.

zoneID

Dictionary that identifies a record zone to monitor in the database.

zoneWide

A Boolean value determining whether all zones should be searched. If `true`, all zones are searched. If `false`, the default zone is searched.

## See Also

### Structures

CloudKit.CloudKitConfig

Dictionary used to configure the CloudKit environment.

CloudKit.ContainerConfig

A configuration for a container.

CloudKit.NameComponents

The parts of the user’s name.

CloudKit.NotificationInfo

Information about a notification.

CloudKit.Query

Search parameters to use when fetching records from the database.

CloudKit.Record

A record in the database.

CloudKit.RecordField

A field value of a record.

CloudKit.RecordInfo

Encapsulates the results of fetching information about a record.

CloudKit.RecordZone

Represents a record zone.

CloudKit.RecordZoneChanges

Represents the changes in a record zone.

CloudKit.RecordZoneChangesOptions

Options about fetching changes in a record zone.

CloudKit.Share

Represents a shared record.

CloudKit.ShareParticipant

Represents a user who accepted a shared record.

CloudKit.SharingUIResult

Represents the results of sharing a record with other users.

CloudKit.UserIdentity

Information to identify a user.

