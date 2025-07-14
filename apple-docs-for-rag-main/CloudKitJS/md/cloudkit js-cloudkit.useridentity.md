

- CloudKit JS
-  CloudKit.UserIdentity 

Structure

# CloudKit.UserIdentity

Information to identify a user.

CloudKit JS 1.0+

``` source
dictionary CloudKit.UserIdentity {
 CloudKit.NameComponents nameComponents;
 String userRecordName;
 CloudKit.UserLookupInfo lookupInfo;
};
```

## Overview

If a user is discoverable, the CloudKit.UserIdentity dictionary contains a `nameComponents` key that you can use to get the user’s first and last name; otherwise, to protect the users’s privacy, the CloudKit.UserIdentity dictionary contains only the `lookupInfo` key.

## Topics

### Instance Properties

lookupInfo

Information used to fetch a user.

nameComponents

An object that contains the user’s name. Use the `familyName` key to get the last name, and the `givenName` key to get the first name.

userRecordName

The name of the user record.

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

CloudKit.Subscription

A subscription, which is a persistent query on the server that tracks the creation, deletion, and modification of records.

