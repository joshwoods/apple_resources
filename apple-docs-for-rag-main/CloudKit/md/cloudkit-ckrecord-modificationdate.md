

- CloudKit
- CKRecord
-  modificationDate 

Instance Property

# modificationDate

The most recent time that CloudKit saved the record to the server.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var modificationDate: Date? { get }
```

## Discussion

The modification date reflects the most recent time that CloudKit saved a record with the current record’s ID to the server. For new instances of this class, the value of this property is initially `nil`. When you save the record to the server, the value updates with the modification date for the record.

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

var lastModifiedUserRecordID: CKRecord.ID?

The ID of the user who most recently modified the record.

var recordChangeTag: String?

The server change token for the record.

class ID

An object that uniquely identifies a record in a database.

