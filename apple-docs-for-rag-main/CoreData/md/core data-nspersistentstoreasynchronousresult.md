

- Core Data
-  NSPersistentStoreAsynchronousResult 

Class

# NSPersistentStoreAsynchronousResult

A concrete class used to represent the results of an asynchronous request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSPersistentStoreAsynchronousResult
```

## Topics

### Inspecting the Result

var managedObjectContext: NSManagedObjectContext

The managed object context for the result.

var operationError: (any Error)?

An error that contains details if the asynchronous fetch request fails.

var progress: Progress?

An object that reports progress for the asynchronous fetch request.

### Canceling the Result

func cancel()

Cancels the asynchronous fetch request.

### Data Types

typealias NSPersistentStoreAsynchronousFetchResultCompletionBlock

A completion block that an asynchronous fetch request calls with a result.

## Relationships

### Inherits From

- NSPersistentStoreResult

### Inherited By

- NSAsynchronousFetchResult

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Store Coordination

class NSPersistentStoreCoordinator

An object that enables an app’s contexts and the underlying persistent stores to work together.

class NSPersistentStore

The abstract base class for all Core Data persistent stores.

class NSPersistentStoreDescription

A description object used to create and load a persistent store.

class NSPersistentStoreRequest

Criteria used to retrieve data from or save data to a persistent store.

class NSPersistentStoreResult

The abstract base class for results returned from a persistent store coordinator.

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

