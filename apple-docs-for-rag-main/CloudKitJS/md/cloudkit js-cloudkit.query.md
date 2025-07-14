

- CloudKit JS
-  CloudKit.Query 

Structure

# CloudKit.Query

Search parameters to use when fetching records from the database.

CloudKit JS 1.0+

``` source
dictionary CloudKit.Query {
 String recordType;
 Object[] filterBy;
 Object[] sortBy;
};
```

## Overview

The `CloudKit.Query` dictionary is the same as the dictionary described in Fetching Records Using a Query (records/query) in CloudKit Web Services Reference.

## Topics

### Instance Properties

filterBy

An array of predicate dictionaries used to determine whether a record matches the query.

recordType

The name of the record type. This key is required.

sortBy

An array of sort descriptor dictionaries that specify how to order the fetched records.

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

CloudKit.Subscription

A subscription, which is a persistent query on the server that tracks the creation, deletion, and modification of records.

CloudKit.UserIdentity

Information to identify a user.

