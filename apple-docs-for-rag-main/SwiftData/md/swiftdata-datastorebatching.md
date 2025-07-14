

- SwiftData
-  DataStoreBatching 

Protocol

# DataStoreBatching

An interface that enables a custom data store to support batch requests.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
protocol DataStoreBatching : DataStore
```

## Topics

### Deleting persisted model data

func delete&lt;T>(DataStoreBatchDeleteRequest&lt;T>) throws

**Required**

struct DataStoreBatchDeleteRequest

## Relationships

### Inherits From

- DataStore

### Conforming Types

- DefaultStore

## See Also

### Model storage

Maintaining a local copy of server data

Create and update a persistent store to cache read-only network data.

class DefaultStore

A data store that uses Core Data as its undelying storage mechanism.

protocol DataStore

An interface that enables SwiftData to read and write model data without knowledge of the underlying storage mechanism.

Building a document-based app using SwiftData

Code along with the WWDC presenter to transform an app with SwiftData.

struct ModelDocument

A document type that uses SwiftData to manage its storage.

