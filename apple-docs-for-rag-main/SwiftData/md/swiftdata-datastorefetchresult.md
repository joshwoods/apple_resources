

- SwiftData
-  DataStoreFetchResult 

Structure

# DataStoreFetchResult

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
struct DataStoreFetchResult where ModelType : PersistentModel, SnapshotType : DataStoreSnapshot
```

## Topics

### Initializers

init(descriptor: FetchDescriptor&lt;ModelType>, fetchedSnapshots: [SnapshotType], relatedSnapshots: [PersistentIdentifier : SnapshotType])

### Instance Properties

let descriptor: FetchDescriptor&lt;ModelType>

let fetchedSnapshots: [SnapshotType]

let relatedSnapshots: [PersistentIdentifier : SnapshotType]

## Relationships

### Conforms To

- Sendable

## See Also

### Processing fetch requests

func fetch&lt;T>(DataStoreFetchRequest&lt;T>) throws -> DataStoreFetchResult&lt;T, Self.Snapshot>

**Required**

struct DataStoreFetchRequest

associatedtype Snapshot : DataStoreSnapshot

**Required**

protocol DataStoreSnapshot

typealias DataStoreSnapshotValue

func fetchCount&lt;T>(DataStoreFetchRequest&lt;T>) throws -> Int

**Required** Default implementation provided.

func fetchIdentifiers&lt;T>(DataStoreFetchRequest&lt;T>) throws -> [PersistentIdentifier]

**Required** Default implementation provided.

