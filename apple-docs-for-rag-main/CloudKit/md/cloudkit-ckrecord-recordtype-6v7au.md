

- CloudKit
- CKRecord
-  recordType 

Instance Property

# recordType

The value that your app defines to identify the type of record.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
var recordType: CKRecord.RecordType { get }
```

## Discussion

Use this value to differentiate between different record types in your app. The value is primarily for your benefit, so choose record types that represent the data in the corresponding records.

CloudKit provides two system-defined record types:

| Record Type | Description |
|----|----|
| CKRecordTypeUserRecord | Identifies records that represent users. |
| CKRecordTypeShare | Identifies records that the user shares. |

## See Also

### Accessing the Record’s Metadata

var recordID: CKRecord.ID

The unique ID of the record.

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

class ID

An object that uniquely identifies a record in a database.

