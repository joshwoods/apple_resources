

- Core Data
-  NSIncrementalStoreNode 

Class

# NSIncrementalStoreNode

A concrete class used to represent basic nodes in a Core Data incremental store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSIncrementalStoreNode
```

## Overview

A node represents a single record in a persistent store.

You can subclass `NSIncrementalStoreNode` to provide custom behavior.

## Topics

### Initializing a Node

init(objectID: NSManagedObjectID, withValues: [String : Any], version: UInt64)

Returns an object initialized with the given values.

### Managing Node Data

var objectID: NSManagedObjectID

The object ID that identifies the data stored by the receiver.

func update(withValues: [String : Any], version: UInt64)

Update the values and version to reflect new data being saved to or loaded from the external store.

func value(for: NSPropertyDescription) -> Any?

Returns the value for the given property.

var version: UInt64

The version of data in the receiver.

## Relationships

### Inherits From

- NSObject

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

