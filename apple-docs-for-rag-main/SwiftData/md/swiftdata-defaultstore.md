

- SwiftData
-  DefaultStore 

Class

# DefaultStore

A data store that uses Core Data as its undelying storage mechanism.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
final class DefaultStore
```

## Mentioned in 

Fetching and filtering time-based model changes

## Topics

### Creating a data store

convenience init(ModelConfiguration, migrationPlan: (any SchemaMigrationPlan.Type)?) throws

### Accessing store information

let configuration: ModelConfiguration

typealias Configuration

var identifier: String

let name: String

let schema: Schema

### Processing fetch requests

func fetch&lt;T>(DataStoreFetchRequest&lt;T>) throws -> DataStoreFetchResult&lt;T, DefaultStore.Snapshot>

typealias Snapshot

struct DefaultSnapshot

func fetchCount&lt;T>(DataStoreFetchRequest&lt;T>) throws -> Int

func fetchIdentifiers&lt;T>(DataStoreFetchRequest&lt;T>) throws -> [PersistentIdentifier]

### Persisting model data

func save(DataStoreSaveChangesRequest&lt;DefaultStore.Snapshot>) throws -> DataStoreSaveChangesResult&lt;DefaultStore.Snapshot>

### Deleting persisted model data

func delete&lt;T>(DataStoreBatchDeleteRequest&lt;T>) throws

func erase() throws

### Sharing cached data between model contexts

func initializeState(for: EditingState)

func cachedSnapshots(for: [PersistentIdentifier], editingState: EditingState) throws -> [PersistentIdentifier : DefaultStore.Snapshot]

func invalidateState(for: EditingState)

### Managing model change history

func fetchHistory(HistoryDescriptor&lt;DefaultHistoryTransaction>) throws -> [DefaultHistoryTransaction]

func deleteHistory(HistoryDescriptor&lt;DefaultHistoryTransaction>) throws

typealias HistoryType

typealias TokenType

### Default Implementations

DataStore Implementations

HistoryProviding Implementations

## Relationships

### Conforms To

- Copyable
- DataStore
- DataStoreBatching
- HistoryProviding

## See Also

### Model storage

Maintaining a local copy of server data

Create and update a persistent store to cache read-only network data.

protocol DataStore

An interface that enables SwiftData to read and write model data without knowledge of the underlying storage mechanism.

protocol DataStoreBatching

An interface that enables a custom data store to support batch requests.

Building a document-based app using SwiftData

Code along with the WWDC presenter to transform an app with SwiftData.

struct ModelDocument

A document type that uses SwiftData to manage its storage.

