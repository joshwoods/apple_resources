

- SwiftData
-  DataStoreSaveChangesRequest 

Structure

# DataStoreSaveChangesRequest

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
struct DataStoreSaveChangesRequest where SnapshotType : DataStoreSnapshot
```

## Topics

### Instance Properties

let deleted: [SnapshotType]

let editingState: EditingState

let inserted: [SnapshotType]

let updated: [SnapshotType]

## Relationships

### Conforms To

- Sendable

## See Also

### Persisting model data

func save(DataStoreSaveChangesRequest&lt;Self.Snapshot>) throws -> DataStoreSaveChangesResult&lt;Self.Snapshot>

**Required**

class DataStoreSaveChangesResult

