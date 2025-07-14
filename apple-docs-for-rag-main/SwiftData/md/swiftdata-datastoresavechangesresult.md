

- SwiftData
-  DataStoreSaveChangesResult 

Class

# DataStoreSaveChangesResult

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
final class DataStoreSaveChangesResult where T : DataStoreSnapshot
```

## Topics

### Initializers

init(for: String, remappedIdentifiers: [PersistentIdentifier : PersistentIdentifier], snapshotsToReregister: [PersistentIdentifier : T])

### Instance Properties

let remappedIdentifiers: [PersistentIdentifier : PersistentIdentifier]

let snapshotsToReregister: [PersistentIdentifier : T]

let storeIdentifier: String

## Relationships

### Conforms To

- Sendable

## See Also

### Persisting model data

func save(DataStoreSaveChangesRequest&lt;Self.Snapshot>) throws -> DataStoreSaveChangesResult&lt;Self.Snapshot>

**Required**

struct DataStoreSaveChangesRequest

