

- CloudKit
- CKSyncEngine
- CKSyncEngine.State
-  pendingDatabaseChanges 

Instance Property

# pendingDatabaseChanges

The database changes that the sync engine has yet to send to the iCloud servers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
final var pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange] { get }
```

## Discussion

This array contains any pending database changes to send to the iCloud servers in a subsequent send operation (scheduled or manual). After the sync engine sends those changes, your app’s sync delegate receives an event of type CKSyncEngine.Event.SentDatabaseChanges.

Use the add(pendingDatabaseChanges:) and remove(pendingDatabaseChanges:) methods to modify the array’s contents.

## See Also

### Accessing pending changes

var hasPendingUntrackedChanges: Bool

A Boolean value that indicates whether there are pending changes that the sync engine is unaware of.

var pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange]

The record zone changes that the sync engine has yet to send to the iCloud servers.

