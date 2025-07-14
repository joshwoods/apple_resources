

- SwiftData
- DataStore
-  fetchCount(\_:) 

Instance Method

# fetchCount(\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
func fetchCount(_ request: DataStoreFetchRequest) throws -> Int where T : PersistentModel
```

**Required** Default implementation provided.

## Default Implementations

### DataStore Implementations

func fetchCount&lt;T>(DataStoreFetchRequest&lt;T>) throws -> Int

## See Also

### Processing fetch requests

func fetch&lt;T>(DataStoreFetchRequest&lt;T>) throws -> DataStoreFetchResult&lt;T, Self.Snapshot>

**Required**

struct DataStoreFetchRequest

struct DataStoreFetchResult

associatedtype Snapshot : DataStoreSnapshot

**Required**

protocol DataStoreSnapshot

typealias DataStoreSnapshotValue

func fetchIdentifiers&lt;T>(DataStoreFetchRequest&lt;T>) throws -> [PersistentIdentifier]

**Required** Default implementation provided.

