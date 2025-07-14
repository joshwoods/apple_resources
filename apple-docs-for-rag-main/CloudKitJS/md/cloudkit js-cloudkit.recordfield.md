

- CloudKit JS
-  CloudKit.RecordField 

Structure

# CloudKit.RecordField

A field value of a record.

CloudKit JS 1.0+

``` source
dictionary CloudKit.RecordField {
 String type;
 Object value;
};
```

## Overview

The `CloudKit.RecordField` dictionary is similar to the dictionary described in Record Field Dictionary in CloudKit Web Services Reference.

## Topics

### Instance Properties

type

The type of the field.

value

The value of the field.

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

