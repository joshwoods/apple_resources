

- SwiftData
- DataStore
-  Snapshot 

Associated Type

# Snapshot

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
associatedtype Snapshot : DataStoreSnapshot
```

**Required**

## See Also

### Processing fetch requests

func fetch&lt;T>(DataStoreFetchRequest&lt;T>) throws -> DataStoreFetchResult&lt;T, Self.Snapshot>

**Required**

struct DataStoreFetchRequest

struct DataStoreFetchResult

protocol DataStoreSnapshot

typealias DataStoreSnapshotValue

func fetchCount&lt;T>(DataStoreFetchRequest&lt;T>) throws -> Int

**Required** Default implementation provided.

func fetchIdentifiers&lt;T>(DataStoreFetchRequest&lt;T>) throws -> [PersistentIdentifier]

**Required** Default implementation provided.

