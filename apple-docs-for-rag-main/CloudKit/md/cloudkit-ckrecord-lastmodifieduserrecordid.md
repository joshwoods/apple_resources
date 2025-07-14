

- CloudKit
- CKRecord
-  lastModifiedUserRecordID 

Instance Property

# lastModifiedUserRecordID

The ID of the user who most recently modified the record.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var lastModifiedUserRecordID: CKRecord.ID? { get }
```

## Discussion

Use this property’s value to retrieve the user record of the user who most recently modified this record. Every user of the app has a unique user record that is empty by default. Apps can add data to the user record on behalf of the user, but don’t store sensitive data in it.

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

var recordChangeTag: String?

The server change token for the record.

class ID

An object that uniquely identifies a record in a database.

