

- Core Data
-  NSAtomicStore 

Class

# NSAtomicStore

An abstract superclass that you subclass to create a Core Data atomic store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSAtomicStore
```

## Overview

Use an atomic store to handle data sets that can be expressed in memory. The atomic store API favors simplicity over performance.

This class provides default implementations of some utility methods. Create a custom atomic store subclass when you have a custom file format that you want to integrate with a Core Data app. When you create a subclass, override the following NSAtomicStore methods:

- load()

- newCacheNode(for:)

- newReferenceObject(for:)

- save()

- updateCacheNode(_:from:)

Also override the following properties and methods of NSPersistentStore, from which the atomic store class inherits:

- type

- identifier

- metadata

- metadataForPersistentStore(with:)

- setMetadata(_:forPersistentStoreAt:)

`NSAtomicStore` provides a default dictionary of metadata. This dictionary contains the store type and identifier (NSStoreTypeKey and NSStoreUUIDKey) as well as store versioning information. Subclasses must ensure that the metadata is saved along with the store data.

## Topics

### Initializing a Store

init(persistentStoreCoordinator: NSPersistentStoreCoordinator?, configurationName: String?, at: URL, options: [AnyHashable : Any]?)

Creates an atomic store at the specified location.

### Loading a Store

func load() throws

Loads the cache nodes for the receiver.

func objectID(for: NSEntityDescription, withReferenceObject: Any) -> NSManagedObjectID

Returns a managed object ID from the reference data for a specified entity.

func addCacheNodes(Set&lt;NSAtomicStoreCacheNode>)

Registers a set of cache nodes with the receiver.

### Updating Cache Nodes

func newCacheNode(for: NSManagedObject) -> NSAtomicStoreCacheNode

Returns a new cache node for a given managed object.

func newReferenceObject(for: NSManagedObject) -> Any

Returns a new reference object for a given managed object.

func updateCacheNode(NSAtomicStoreCacheNode, from: NSManagedObject)

Updates the given cache node using the values in a given managed object.

func willRemoveCacheNodes(Set&lt;NSAtomicStoreCacheNode>)

Method invoked before the store removes the given collection of cache nodes.

### Saving a Store

func save() throws

Saves the cache nodes.

### Utility Methods

func cacheNodes() -> Set&lt;NSAtomicStoreCacheNode>

Returns the set of cache nodes registered with the receiver.

func cacheNode(for: NSManagedObjectID) -> NSAtomicStoreCacheNode?

Returns the cache node for a given managed object ID.

func referenceObject(for: NSManagedObjectID) -> Any

Returns the reference object for a given managed object ID.

## Relationships

### Inherits From

- NSPersistentStore

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

class NSAtomicStoreCacheNode

A concrete class that you use to represent basic nodes in a Core Data atomic store.

class NSIncrementalStore

An abstract superclass defining the API through which Core Data communicates with a store.

class NSIncrementalStoreNode

A concrete class used to represent basic nodes in a Core Data incremental store.

