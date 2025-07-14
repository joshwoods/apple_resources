

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.SentRecordZoneChanges
-  CKSyncEngine.Event.SentRecordZoneChanges.FailedRecordSave 

Structure

# CKSyncEngine.Event.SentRecordZoneChanges.FailedRecordSave

A type that describes an unsuccessful attempt to modify a single record.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct FailedRecordSave
```

## Topics

### Accessing the record

let record: CKRecord

The record that CloudKit is unable to modify.

### Accessing the error

let error: CKError

A error that describes the reason for the unsuccessful attempt to modify the associated record.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Accessing failed changes

let failedRecordDeletes: [CKRecord.ID : CKError]

The unique identifiers of the records CloudKit is unable to delete, and the reasons why.

let failedRecordSaves: [CKSyncEngine.Event.SentRecordZoneChanges.FailedRecordSave]

The records that CloudKit is unable to modify.

