

- CloudKit
- CKSyncEngine
- CKSyncEngine.RecordZoneChangeBatch
-  init(recordsToSave:recordIDsToDelete:atomicByZone:) 

Initializer

# init(recordsToSave:recordIDsToDelete:atomicByZone:)

Creates a batch of records to modify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
init(
    recordsToSave: [CKRecord] = [],
    recordIDsToDelete: [CKRecord.ID] = [],
    atomicByZone: Bool = false
)
```

## Parameters 

`recordsToSave`  

The records to save.

`recordIDsToDelete`  

The identifiers of the records to delete.

`atomicByZone`  

A Boolean value that determines whether CloudKit modifies the specified records atomically by record zone.

## Discussion

Important

When using this initializer to create batches, consider the number of records you specify and their combined size. If you specify too many records, or their combined size is too large, the send operation may fail with an error of type CKError.Code.limitExceeded.

## See Also

### Creating a batch

init?(pendingChanges: [CKSyncEngine.PendingRecordZoneChange], recordProvider: (CKRecord.ID) async -> CKRecord?) async

Creates a batch of records to modify using the provided record zone changes.

enum PendingRecordZoneChange

Describes an unsent record modification.

