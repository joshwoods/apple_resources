

- CloudKit JS
-  CloudKit.Record 

Structure

# CloudKit.Record

A record in the database.

CloudKit JS 1.0+

``` source
dictionary CloudKit.Record {
 Object created;
 Object modified;
 String recordType;
 String recordName;
 String recordChangeTag;
 Boolean deleted;
 Boolean createShortGUID;
 String shortGUID;
 CKReference parent;
 CKReference share;
 Object fields;
};
```

## Overview

The `CloudKit.Record` dictionary is the same as the dictionary described in Modifying Records (records/modify) in CloudKit Web Services Reference.

## Topics

### Instance Properties

createShortGUID

A Boolean value indicating whether to create a short GUID.

created

Information about when the record was created on the server. The properties of this object are: `timestamp` (`Number`), the time at which the record was created, and `user` (`String`), the ID of the user who created the record. This field is used by the CloudKit.RecordsResponse class. The value of this field is set by the server. Omit this key when saving a record.

deleted

A Boolean value indicating whether the record was deleted. `true` if the record was deleted; otherwise, `false`.

fields

Names of the fields or field-value pairs.

modified

Information about when the record was last modified. The properties of this object are: `timestamp` (`Number`), the time at which the record was created, and `user` (`String`), the ID of the user who modified the record. This field is used by the CloudKit.RecordsResponse class. This value of this field is set by the server. Omit this key when saving a record.

parent

A reference to a parent object used for sharing.

recordChangeTag

A string containing the server change token for the record. Use this tag to indicate which version of the record you last fetched. This key is required if you are saving an existing record.

recordName

The unique name used to identify the record. The default value is a random UUID.

recordType

The name of the record type. This key is required if the record doesn’t exist.

share

A reference to the shared object for this record.

shortGUID

A global unique identifier for this record used for sharing.

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

