

- CloudKit JS
-  CloudKit.RecordZoneChanges 

Structure

# CloudKit.RecordZoneChanges

Represents the changes in a record zone.

CloudKit JS 1.0+

``` source
dictionary CloudKit.RecordZoneChanges {
 CloudKit.ZoneID zoneID;
 Boolean resultsLimit;
 String[] desiredKeys;
 String[] desiredRecordTypes;
 Boolean moreComing;
 String syncToken;
 CloudKit.Record[] records;
 CloudKit.CKError[] errors;
};
```

## Topics

### Instance Properties

desiredKeys

An array of record field names that limit the amount of data returned. Only the fields specified in the array are returned. The default is `null`, which fetches all record fields.

desiredRecordTypes

An array of record types that limit the amount of records returned. Only the record types specified in the array are returned.

errors

Errors that may have occurred fetching the changed records.

moreComing

Boolean value that indicates whether there are more changes to request. If `moreComing` is `true`, request more changes using the value of the included `syncToken` key. If `moreComing` is `false`, there are no more changes.

records

The records that changed.

resultsLimit

The maximum number of records to fetch.

syncToken

Identifies a point in the zone’s change history. The first time you get record changes, omit this key and if `moreComing` is `true` in the response, use the `syncToken` in the response in the next request until `moreComing` is `false`. Otherwise, get the current sync token by fetching a zone.

zoneID

The record zone identifier.

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

CloudKit.RecordZoneChangesOptions

Options about fetching changes in a record zone.

CloudKit.Share

Represents a shared record.

CloudKit.ShareParticipant

Represents a user who accepted a shared record.

CloudKit.SharingUIResult

Represents the results of sharing a record with other users.

CloudKit.Subscription

A subscription, which is a persistent query on the server that tracks the creation, deletion, and modification of records.

CloudKit.UserIdentity

Information to identify a user.

