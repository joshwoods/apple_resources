

- CloudKit JS
-  CloudKit.ShareParticipant 

Structure

# CloudKit.ShareParticipant

Represents a user who accepted a shared record.

CloudKit JS 1.0+

``` source
dictionary CloudKit.ShareParticipant {
 CloudKit.ShareParticipantPermission permission;
 CloudKit.ShareParticipantAcceptanceStatus acceptanceStatus;
 CloudKit.ShareParticipantType type;
};
```

## Topics

### Instance Properties

acceptanceStatus

Indicates the status of accepting the shared record.

permission

The participant’s read and write permissions.

type

Type of participant.

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

CloudKit.SharingUIResult

Represents the results of sharing a record with other users.

CloudKit.Subscription

A subscription, which is a persistent query on the server that tracks the creation, deletion, and modification of records.

CloudKit.UserIdentity

Information to identify a user.

