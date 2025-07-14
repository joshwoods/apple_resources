

- CloudKit
- CKModifyRecordsOperation
-  CKModifyRecordsOperation.RecordSavePolicy 

Enumeration

# CKModifyRecordsOperation.RecordSavePolicy

Constants that indicate which policy to apply when saving records.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
enum RecordSavePolicy
```

## Topics

### Save Policies

case ifServerRecordUnchanged

A policy that instructs CloudKit to only proceed if the record’s change tag matches that of the server’s copy.

case changedKeys

A policy that instructs CloudKit to save only the fields of a record that contain changes.

case allKeys

A policy that instructs CloudKit to save all keys of a record, even those without changes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Modifying Records

func modifyRecords(saving: [CKRecord], deleting: [CKRecord.ID], savePolicy: CKModifyRecordsOperation.RecordSavePolicy, atomically: Bool) async throws -> (saveResults: [CKRecord.ID : Result&lt;CKRecord, any Error>], deleteResults: [CKRecord.ID : Result&lt;Void, any Error>])

Modifies the specified records and returns the results to an awaiting caller.

func modifyRecords(saving: [CKRecord], deleting: [CKRecord.ID], savePolicy: CKModifyRecordsOperation.RecordSavePolicy, atomically: Bool, completionHandler: (Result&lt;(saveResults: [CKRecord.ID : Result&lt;CKRecord, any Error>], deleteResults: [CKRecord.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified records and delivers the results to a completion hander.

func save(CKRecord, completionHandler: (CKRecord?, (any Error)?) -> Void)

Saves a specific record.

func delete(withRecordID: CKRecord.ID, completionHandler: (CKRecord.ID?, (any Error)?) -> Void)

Deletes a specific record.

