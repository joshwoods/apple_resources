

- CloudKit
- CKRecord
-  creationDate 

Instance Property

# creationDate

The time when CloudKit first saves the record to the server.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var creationDate: Date? { get }
```

## Discussion

The creation date reflects the time when CloudKit creates a record on the server with the current record’s ID. For new instances of this class, the value of this property is initially `nil`. When you save the record to the server, the value updates with the creation date for the record.

## See Also

### Accessing the Record’s Metadata

var recordID: CKRecord.ID

The unique ID of the record.

var recordType: CKRecord.RecordType

The value that your app defines to identify the type of record.

enum SystemType

Possible values for record types of system records.

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

