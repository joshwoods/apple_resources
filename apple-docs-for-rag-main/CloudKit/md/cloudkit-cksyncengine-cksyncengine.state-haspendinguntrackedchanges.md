

- CloudKit
- CKSyncEngine
- CKSyncEngine.State
-  hasPendingUntrackedChanges 

Instance Property

# hasPendingUntrackedChanges

A Boolean value that indicates whether there are pending changes that the sync engine is unaware of.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
final var hasPendingUntrackedChanges: Bool { get set }
```

## Discussion

Use this property to inform the sync engine that there are pending changes other than those available in pendingRecordZoneChanges. After you set this property, the sync engine automatically schedules a send operation and, when that operation executes, asks your delegate to provide those changes by invoking the nextRecordZoneChangeBatch(_:syncEngine:) method.

Using this property is optional and is necessary only if you track pending changes manually, outside of the sync engine’s state.

## See Also

### Accessing pending changes

var pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange]

The database changes that the sync engine has yet to send to the iCloud servers.

var pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange]

The record zone changes that the sync engine has yet to send to the iCloud servers.

