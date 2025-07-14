

- SwiftData
-  DataStoreSnapshot 

Protocol

# DataStoreSnapshot

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
protocol DataStoreSnapshot : Decodable, Encodable, Sendable
```

## Topics

### Initializers

init(from: any BackingData, relatedBackingDatas: inout [PersistentIdentifier : any BackingData])

**Required**

### Instance Properties

var persistentIdentifier: PersistentIdentifier

**Required**

### Instance Methods

func copy(persistentIdentifier: PersistentIdentifier, remappedIdentifiers: [PersistentIdentifier : PersistentIdentifier]?) -> Self

**Required**

## Relationships

### Inherits From

- Decodable
- Encodable
- Sendable

### Conforming Types

- DefaultSnapshot

## See Also

### Processing fetch requests

func fetch&lt;T>(DataStoreFetchRequest&lt;T>) throws -> DataStoreFetchResult&lt;T, Self.Snapshot>

**Required**

struct DataStoreFetchRequest

struct DataStoreFetchResult

associatedtype Snapshot : DataStoreSnapshot

**Required**

typealias DataStoreSnapshotValue

func fetchCount&lt;T>(DataStoreFetchRequest&lt;T>) throws -> Int

**Required** Default implementation provided.

func fetchIdentifiers&lt;T>(DataStoreFetchRequest&lt;T>) throws -> [PersistentIdentifier]

**Required** Default implementation provided.

