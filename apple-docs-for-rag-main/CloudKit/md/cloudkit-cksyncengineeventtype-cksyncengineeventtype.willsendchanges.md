

- CloudKit
- CKSyncEngineEventType
-  CKSyncEngineEventType.willSendChanges 

Case

# CKSyncEngineEventType.willSendChanges

An event indicating an imminent send of local changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case willSendChanges
```

## See Also

### Event types

case stateUpdate

An event indicating an update to the sync engine’s state.

case accountChange

An event indicating a change to the device’s iCloud account.

case fetchedDatabaseChanges

An event indicating there are fetched database changes to process.

case fetchedRecordZoneChanges

An event indicating there are fetched record zone changes to process.

case sentDatabaseChanges

An event indicating a sent batch of database changes.

case sentRecordZoneChanges

An event indicating a sent batch of record zone changes.

case willFetchChanges

An event indicating an imminent database fetch.

case willFetchRecordZoneChanges

An event indicating an imminent fetch of changes in a record zone.

case didFetchRecordZoneChanges

An event that indicates the record zone fetch is done.

case didFetchChanges

An event that indicates the database fetch is done.

case didSendChanges

An event that indicates a finished send operation.

