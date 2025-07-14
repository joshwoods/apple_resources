

- CloudKit
- CKRecord
-  CKRecord.SystemType 

Enumeration

# CKRecord.SystemType

Possible values for record types of system records.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
enum SystemType
```

## Topics

### Types of System Records

static let share: CKRecord.RecordType

A string that represents the record type for CloudKit share records.

static let userRecord: CKRecord.RecordType

A string that represents the record type for CloudKit user records.

## See Also

### Accessing the Record’s Metadata

var recordID: CKRecord.ID

The unique ID of the record.

var recordType: CKRecord.RecordType

The value that your app defines to identify the type of record.

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

class ID

An object that uniquely identifies a record in a database.

