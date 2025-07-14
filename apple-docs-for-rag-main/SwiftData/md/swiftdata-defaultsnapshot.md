

- SwiftData
-  DefaultSnapshot 

Structure

# DefaultSnapshot

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
struct DefaultSnapshot
```

## Topics

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(from: any BackingData, relatedBackingDatas: inout [PersistentIdentifier : any BackingData])

### Instance Properties

let persistentIdentifier: PersistentIdentifier

### Instance Methods

func copy(persistentIdentifier: PersistentIdentifier, remappedIdentifiers: [PersistentIdentifier : PersistentIdentifier]?) -> DefaultSnapshot

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

## Relationships

### Conforms To

- DataStoreSnapshot
- Decodable
- Encodable
- Sendable

## See Also

### Processing fetch requests

func fetch&lt;T>(DataStoreFetchRequest&lt;T>) throws -> DataStoreFetchResult&lt;T, DefaultStore.Snapshot>

typealias Snapshot

func fetchCount&lt;T>(DataStoreFetchRequest&lt;T>) throws -> Int

func fetchIdentifiers&lt;T>(DataStoreFetchRequest&lt;T>) throws -> [PersistentIdentifier]

