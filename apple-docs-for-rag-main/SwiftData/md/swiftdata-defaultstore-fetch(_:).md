

- SwiftData
- DefaultStore
-  fetch(\_:) 

Instance Method

# fetch(\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
final func fetch(_ request: DataStoreFetchRequest) throws -> DataStoreFetchResult where T : PersistentModel
```

## See Also

### Processing fetch requests

typealias Snapshot

struct DefaultSnapshot

func fetchCount&lt;T>(DataStoreFetchRequest&lt;T>) throws -> Int

func fetchIdentifiers&lt;T>(DataStoreFetchRequest&lt;T>) throws -> [PersistentIdentifier]

