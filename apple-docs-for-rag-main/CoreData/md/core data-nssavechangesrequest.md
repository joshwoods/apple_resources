

- Core Data
-  NSSaveChangesRequest 

Class

# NSSaveChangesRequest

An encapsulation of a collection of changes to be made by an object store in response to a save operation on a managed object context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSSaveChangesRequest
```

## Topics

### Initializing a Request

init(inserted: Set&lt;NSManagedObject>?, updated: Set&lt;NSManagedObject>?, deleted: Set&lt;NSManagedObject>?, locked: Set&lt;NSManagedObject>?)

Initializes a save changes request with collections of given changes.

### Getting Information about a Request

var insertedObjects: Set&lt;NSManagedObject>?

The objects that were inserted into the calling context.

var updatedObjects: Set&lt;NSManagedObject>?

The objects that were modified in the calling context.

var deletedObjects: Set&lt;NSManagedObject>?

The objects that were deleted in the calling context.

var lockedObjects: Set&lt;NSManagedObject>?

The objects that were flagged for optimistic locking on the calling context.

## Relationships

### Inherits From

- NSPersistentStoreRequest

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

class NSPersistentStoreRequest

Criteria used to retrieve data from or save data to a persistent store.

class NSPersistentStoreResult

The abstract base class for results returned from a persistent store coordinator.

class NSPersistentStoreAsynchronousResult

A concrete class used to represent the results of an asynchronous request.

class NSAtomicStore

An abstract superclass that you subclass to create a Core Data atomic store.

class NSAtomicStoreCacheNode

A concrete class that you use to represent basic nodes in a Core Data atomic store.

class NSIncrementalStore

An abstract superclass defining the API through which Core Data communicates with a store.

class NSIncrementalStoreNode

A concrete class used to represent basic nodes in a Core Data incremental store.

