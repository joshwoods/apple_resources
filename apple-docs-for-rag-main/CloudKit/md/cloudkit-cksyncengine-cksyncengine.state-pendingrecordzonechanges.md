

- CloudKit
- CKSyncEngine
- CKSyncEngine.State
-  pendingRecordZoneChanges 

Instance Property

# pendingRecordZoneChanges

The record zone changes that the sync engine has yet to send to the iCloud servers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
final var pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange] { get }
```

## Discussion

This array contains any pending record zone changes to send to the iCloud servers in a subsequent send operation (scheduled or manual). After the sync engine sends those changes, your app’s sync delegate receives an event of type CKSyncEngine.Event.SentRecordZoneChanges.

Use the add(pendingRecordZoneChanges:) and remove(pendingRecordZoneChanges:) methods to modify the array’s contents.

## See Also

### Accessing pending changes

var hasPendingUntrackedChanges: Bool

A Boolean value that indicates whether there are pending changes that the sync engine is unaware of.

var pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange]

The database changes that the sync engine has yet to send to the iCloud servers.

