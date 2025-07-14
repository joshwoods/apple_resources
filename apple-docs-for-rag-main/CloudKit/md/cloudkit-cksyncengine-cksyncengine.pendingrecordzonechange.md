

- CloudKit
- CKSyncEngine
-  CKSyncEngine.PendingRecordZoneChange 

Enumeration

# CKSyncEngine.PendingRecordZoneChange

Describes an unsent record modification.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
enum PendingRecordZoneChange
```

## Topics

### Record change types

enum CKSyncEnginePendingRecordZoneChangeType

Describes a type of modification a record zone change makes.

### Enumeration Cases

case deleteRecord(CKRecord.ID)

case saveRecord(CKRecord.ID)

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

enum PendingDatabaseChange

Describes an unsent database modification.

func add(pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange])

Adds the specified record zone changes to the state.

func remove(pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange])

Removes the specified record zone changes from the state.

