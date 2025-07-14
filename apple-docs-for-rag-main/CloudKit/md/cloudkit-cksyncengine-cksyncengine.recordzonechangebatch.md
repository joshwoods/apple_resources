

- CloudKit
- CKSyncEngine
-  CKSyncEngine.RecordZoneChangeBatch 

Structure

# CKSyncEngine.RecordZoneChangeBatch

A type that contains the record changes for a single send operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct RecordZoneChangeBatch
```

## Topics

### Creating a batch

init?(pendingChanges: [CKSyncEngine.PendingRecordZoneChange], recordProvider: (CKRecord.ID) async -> CKRecord?) async

Creates a batch of records to modify using the provided record zone changes.

enum PendingRecordZoneChange

Describes an unsent record modification.

init(recordsToSave: [CKRecord], recordIDsToDelete: [CKRecord.ID], atomicByZone: Bool)

Creates a batch of records to modify.

### Managing atomicity

var atomicByZone: Bool

A Boolean value that determines whether CloudKit modifies records atomically by record zone.

### Managing the records

var recordIDsToDelete: [CKRecord.ID]

The record identifiers of the records to delete.

var recordsToSave: [CKRecord]

The records to save.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Sending changes

func nextRecordZoneChangeBatch(CKSyncEngine.SendChangesContext, syncEngine: CKSyncEngine) async -> CKSyncEngine.RecordZoneChangeBatch?

Asks the delegate to provide the next set of record changes to send to the server.

**Required**

struct SendChangesContext

A type that describes a single attempt to send changes to the iCloud servers.

