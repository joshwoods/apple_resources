

- CloudKit
- CKSyncEngine
- CKSyncEngine.State
-  add(pendingDatabaseChanges:) 

Instance Method

# add(pendingDatabaseChanges:)

Adds the specified database changes to the state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
final func add(pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange])
```

## Parameters 

`pendingDatabaseChanges`  

An array of database changes.

## Discussion

Use this method to enable the sync engine to manage your pending database changes. For example, when someone makes a change that your app needs to send to the server, use this method to record the change. If there are no scheduled sync operations when you invoke this method, the sync engine automatically schedules one to send the changes. After the engine sends those changes, it notifies your app’s sync delegate with an event of type CKSyncEngine.Event.SentDatabaseChanges.

The sync engine ensures the consistency of any pending changes it’s tracking, deduplicating them as necessary. The engine removes changes from the list as it sends them, but retains any that fail due to a recoverable error, such as a network issue or exceeding the rate limit.

Note

The order in which you apply database changes is important. For example, if you add a save change and then a delete change, the sync engine discards the save and sends only the delete change. The reverse is also true.

## See Also

### Manipulating pending changes

func remove(pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange])

Removes the specified database changes from the state.

enum PendingDatabaseChange

Describes an unsent database modification.

func add(pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange])

Adds the specified record zone changes to the state.

func remove(pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange])

Removes the specified record zone changes from the state.

enum PendingRecordZoneChange

Describes an unsent record modification.

