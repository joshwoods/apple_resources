

- CloudKit
- CKSyncEngine
- CKSyncEngine.RecordZoneChangeBatch
-  init(pendingChanges:recordProvider:) 

Initializer

# init(pendingChanges:recordProvider:)

Creates a batch of records to modify using the provided record zone changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
init?(
    pendingChanges: [CKSyncEngine.PendingRecordZoneChange],
    recordProvider: (CKRecord.ID) async -> CKRecord?
) async
```

## Parameters 

`pendingChanges`  

The record zone changes to process.

`recordProvider`  

A closure that returns the record for the specified record identifier.

## Return Value

The batch of records to modify, or `nil` if there are no pending changes.

## Discussion

This method iterates over `pendingChanges` and adds the necessary information to the new batch, until there are no more changes or the size of the batch reaches the maximum limit. If the type of change is a record save, the method asks the specified `recordProvider` closure for that record. If the closure returns `nil`, the method skips that change.

## See Also

### Creating a batch

enum PendingRecordZoneChange

Describes an unsent record modification.

init(recordsToSave: [CKRecord], recordIDsToDelete: [CKRecord.ID], atomicByZone: Bool)

Creates a batch of records to modify.

