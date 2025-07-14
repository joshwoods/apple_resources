

- CloudKit
- CKSyncEngineDelegate
-  nextRecordZoneChangeBatch(\_:syncEngine:) 

Instance Method

# nextRecordZoneChangeBatch(\_:syncEngine:)

Asks the delegate to provide the next set of record changes to send to the server.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func nextRecordZoneChangeBatch(
    _ context: CKSyncEngine.SendChangesContext,
    syncEngine: CKSyncEngine
) async -> CKSyncEngine.RecordZoneChangeBatch?
```

**Required**

## Parameters 

`context`  

The reason for the sync engine’s request, and any additional options that request is using.

`syncEngine`  

The sync engine asking about pending changes.

## Return Value

If there are pending record changes, a batch of those changes for the sync engine to process; otherwise, `nil` to indicate there are no changes to send.

## Discussion

In your implementation, ask the sync engine’s state for any pending record zone changes and then return a change batch containing a CKRecord instance for each record identifier the state provides, as the following example shows:

```
func nextRecordZoneChangeBatch(
    _ context: CKSyncEngine.SendChangesContext, 
    syncEngine: CKSyncEngine
) async -> CKSyncEngine.RecordZoneChangeBatch? {

    // Get the pending record changes and filter by the context's scope.
    let pendingChanges = syncEngine.state.pendingRecordZoneChanges
        .filter { context.options.zoneIDs.contains($0) }

    // Return a change batch that contains the corresponding materialized records.
    return await CKSyncEngine.RecordZoneChangeBatch(
        pendingChanges: pendingChanges) { self.recordFor(id: $0) }
}
```

For both scheduled and manual send operations, the sync engine calls this method repeatedly until your app has no more changes and returns `nil`.

## See Also

### Sending changes

struct SendChangesContext

A type that describes a single attempt to send changes to the iCloud servers.

struct RecordZoneChangeBatch

A type that contains the record changes for a single send operation.

