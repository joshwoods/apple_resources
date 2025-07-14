

- CloudKit
- CKSyncEngine
-  CKSyncEngine.PendingDatabaseChange 

Enumeration

# CKSyncEngine.PendingDatabaseChange

Describes an unsent database modification.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
enum PendingDatabaseChange
```

## Topics

### Database change types

enum CKSyncEnginePendingDatabaseChangeType

Describes the type of a pending database change.

### Enumeration Cases

case deleteZone(CKRecordZone.ID)

case saveZone(CKRecordZone)

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Manipulating pending changes

func add(pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange])

Adds the specified database changes to the state.

func remove(pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange])

Removes the specified database changes from the state.

func add(pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange])

Adds the specified record zone changes to the state.

func remove(pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange])

Removes the specified record zone changes from the state.

enum PendingRecordZoneChange

Describes an unsent record modification.

