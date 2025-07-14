

- CloudKit
- CKRecord
-  CKRecord.ID 

Class

# CKRecord.ID

An object that uniquely identifies a record in a database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class ID
```

## Overview

A record ID object consists of a name string and a zone ID. The name string is an ASCII string that doesn’t exceed 255 characters in length. For automatically created records, the ID name string derives from a UUID and is, therefore, unique. When creating your own record ID objects, you can use names that have more meaning to your app or to the user, as long as each name is unique within the specified zone. For example, you might use a document name for the name string.

Record IDs must be unique within the specified database, but you can reuse record IDs in different databases. Each container has a public and a private database, and the private database is different for each unique user. This configuration provides for the reusing of record IDs in each user’s private database, but ensures that only one record uses a specific record ID in the public database.

CloudKit generally creates record IDs when it first saves a new record, but you might manually instantiate instances of `CKRecordID` in specific situations. For example, you must create an instance when saving a record in a zone other than the default zone. You also instantiate instances of `CKRecordID` when retrieving specific records from a database.

Don’t subclass `CKRecordID`.

### Interacting with Record IDs

After you create a `CKRecordID` object, interactions with that object typically involve creating a new record or retrieving an existing record from a database.

You might also use record IDs when you can’t use a CKRecord.Reference object to refer to a record. References are only valid within a single zone of a database. To refer to objects outside of the current zone or database, save the strings in the record’s `CKRecordID` and CKRecordZone.ID objects. When you want to retrieve the record later, use those strings to recreate the record and zone ID objects so that you can fetch the record.

#### Creating Record IDs for New Records

To assign a custom record ID to a new record, you must create the `CKRecordID` object first. You need to know the intended name and zone information for that record, which might also require creating a CKRecordZone.ID object. After creating the record ID object, initialize your new record using its initWithRecordType:recordID: method.

#### Using Record IDs to Fetch Records

Use a record ID to fetch the corresponding CKRecord object from a database quickly. You perform the fetch operation using a CKFetchRecordsOperation object or the fetch(withRecordID:completionHandler:) method of the CKDatabase class. In both cases, CloudKit returns the record asynchronously using the handler you provide.

## Topics

### Creating a Record ID

convenience init(recordName: String)

Creates a new record ID with the specified name in the default zone.

convenience init(recordName: String, zoneID: CKRecordZone.ID)

Creates a new record ID with the specified name and zone information.

let CKRecordNameZoneWideShare: String

The name of a share record that manages a shared record zone.

### Getting the Record ID’s Name

var recordName: String

The unique name of the record.

### Getting the Record ID’s Zone

var zoneID: CKRecordZone.ID

The ID of the zone that contains the record.

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

### Accessing the Record’s Metadata

var recordID: CKRecord.ID

The unique ID of the record.

var recordType: CKRecord.RecordType

The value that your app defines to identify the type of record.

enum SystemType

Possible values for record types of system records.

var creationDate: Date?

The time when CloudKit first saves the record to the server.

var creatorUserRecordID: CKRecord.ID?

The ID of the user who creates the record.

var modificationDate: Date?

The most recent time that CloudKit saved the record to the server.

var lastModifiedUserRecordID: CKRecord.ID?

The ID of the user who most recently modified the record.

var recordChangeTag: String?

The server change token for the record.

