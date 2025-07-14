

- SwiftData
- DefaultStore
-  DefaultStore.Snapshot 

Type Alias

# DefaultStore.Snapshot

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
typealias Snapshot = DefaultSnapshot
```

## See Also

### Processing fetch requests

func fetch&lt;T>(DataStoreFetchRequest&lt;T>) throws -> DataStoreFetchResult&lt;T, DefaultStore.Snapshot>

struct DefaultSnapshot

func fetchCount&lt;T>(DataStoreFetchRequest&lt;T>) throws -> Int

func fetchIdentifiers&lt;T>(DataStoreFetchRequest&lt;T>) throws -> [PersistentIdentifier]

