

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.SentRecordZoneChanges 

Structure

# CKSyncEngine.Event.SentRecordZoneChanges

A type that provides information about a sent batch of record zone changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct SentRecordZoneChanges
```

## Topics

### Accessing successful changes

let deletedRecordIDs: [CKRecord.ID]

The unique identifiers of the deleted records.

let savedRecords: [CKRecord]

The modified records.

### Accessing failed changes

let failedRecordDeletes: [CKRecord.ID : CKError]

The unique identifiers of the records CloudKit is unable to delete, and the reasons why.

let failedRecordSaves: [CKSyncEngine.Event.SentRecordZoneChanges.FailedRecordSave]

The records that CloudKit is unable to modify.

struct FailedRecordSave

A type that describes an unsuccessful attempt to modify a single record.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Pending local changes

case willSendChanges(CKSyncEngine.Event.WillSendChanges)

An event indicating an imminent send of local changes.

struct WillSendChanges

A type that provides information about an imminent send of local changes.

case sentDatabaseChanges(CKSyncEngine.Event.SentDatabaseChanges)

An event indicating a sent batch of database changes.

struct SentDatabaseChanges

A type that provides information about a sent batch of database changes.

case sentRecordZoneChanges(CKSyncEngine.Event.SentRecordZoneChanges)

An event indicating a sent batch of record zone changes.

case didSendChanges(CKSyncEngine.Event.DidSendChanges)

An event that indicates a finished send operation.

struct DidSendChanges

A type that provides information about a finished send operation.

