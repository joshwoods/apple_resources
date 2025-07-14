

- Core Data
-  NSPersistentStoreRequest 

Class

# NSPersistentStoreRequest

Criteria used to retrieve data from or save data to a persistent store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSPersistentStoreRequest
```

## Topics

### Configuring a Request

var affectedStores: [NSPersistentStore]?

The stores the request should be sent to.

var requestType: NSPersistentStoreRequestType

The type of the fetch request.

enum NSPersistentStoreRequestType

Constants that specify the types of fetch requests.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSAsynchronousFetchRequest
- NSBatchDeleteRequest
- NSBatchInsertRequest
- NSBatchUpdateRequest
- NSFetchRequest
- NSPersistentCloudKitContainerEventRequest
- NSPersistentHistoryChangeRequest
- NSSaveChangesRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Store Coordination

class NSPersistentStoreCoordinator

An object that enables an app’s contexts and the underlying persistent stores to work together.

class NSPersistentStore

The abstract base class for all Core Data persistent stores.

class NSPersistentStoreDescription

A description object used to create and load a persistent store.

class NSPersistentStoreResult

The abstract base class for results returned from a persistent store coordinator.

class NSPersistentStoreAsynchronousResult

A concrete class used to represent the results of an asynchronous request.

class NSSaveChangesRequest

An encapsulation of a collection of changes to be made by an object store in response to a save operation on a managed object context.

class NSAtomicStore

An abstract superclass that you subclass to create a Core Data atomic store.

class NSAtomicStoreCacheNode

A concrete class that you use to represent basic nodes in a Core Data atomic store.

class NSIncrementalStore

An abstract superclass defining the API through which Core Data communicates with a store.

class NSIncrementalStoreNode

A concrete class used to represent basic nodes in a Core Data incremental store.

