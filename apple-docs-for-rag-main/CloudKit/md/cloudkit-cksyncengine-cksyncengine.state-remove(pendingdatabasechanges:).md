

- CloudKit
- CKSyncEngine
- CKSyncEngine.State
-  remove(pendingDatabaseChanges:) 

Instance Method

# remove(pendingDatabaseChanges:)

Removes the specified database changes from the state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
final func remove(pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange])
```

## Parameters 

`pendingDatabaseChanges`  

An array of database changes.

## See Also

### Manipulating pending changes

func add(pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange])

Adds the specified database changes to the state.

enum PendingDatabaseChange

Describes an unsent database modification.

func add(pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange])

Adds the specified record zone changes to the state.

func remove(pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange])

Removes the specified record zone changes from the state.

enum PendingRecordZoneChange

Describes an unsent record modification.

