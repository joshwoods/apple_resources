

- Core Data
-  NSIncrementalStore 

Class

# NSIncrementalStore

An abstract superclass defining the API through which Core Data communicates with a store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSIncrementalStore
```

## Overview

You use this interface to create persistent stores that load and save data incrementally, allowing for the management of large and/or shared datasets.

### Subclassing Notes

#### Methods to Override

In a subclass of `NSIncrementalStore`, you *must* override the following methods to provide behavior appropriate for your store:

- loadMetadata()

- execute(_:with:)

- newValuesForObject(with:with:)

- newValue(forRelationship:forObjectWith:with:)

- obtainPermanentIDs(for:)

You can also optionally override the following methods:

- identifierForNewStore(at:)

- managedObjectContextDidRegisterObjects(with:)

- managedObjectContextDidUnregisterObjects(with:)

There is no need to override the methods that you must otherwise override for a subclass of NSPersistentStore.

#### Methods that Should Not Be Overridden

In a subclass of `NSIncrementalStore`, you should not override the following methods:

- newObjectID(for:referenceObject:)

- referenceObject(for:)

## Topics

### Manipulating Managed Objects

func execute(NSPersistentStoreRequest, with: NSManagedObjectContext?) throws -> Any

Returns a value as appropriate for the given request, or nil if the request cannot be completed.

func newValuesForObject(with: NSManagedObjectID, with: NSManagedObjectContext) throws -> NSIncrementalStoreNode

Returns an incremental store node encapsulating the persistent external values of the object with a given object ID.

func newValue(forRelationship: NSRelationshipDescription, forObjectWith: NSManagedObjectID, with: NSManagedObjectContext?) throws -> Any

Returns the relationship for the given relationship of the object with a given object ID.

func obtainPermanentIDs(for: [NSManagedObject]) throws -> [NSManagedObjectID]

Returns an array containing the object IDs for a given array of newly-inserted objects.

func newObjectID(for: NSEntityDescription, referenceObject: Any) -> NSManagedObjectID

Returns a new object ID that uses given data as the key.

func referenceObject(for: NSManagedObjectID) -> Any

Returns the reference data used to construct a given object ID.

### Responding to Context Changes

func managedObjectContextDidRegisterObjects(with: [NSManagedObjectID])

Indicates that objects identified by a given array of object IDs are in use in a managed object context.

func managedObjectContextDidUnregisterObjects(with: [NSManagedObjectID])

Indicates that objects identified by a given array of object IDs are no longer being used by a managed object context.

### Accessing Metadata

class func identifierForNewStore(at: URL) -> Any

Returns the identifier for the store at a given URL.

func loadMetadata() throws

Loads the metadata for the store.

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

class NSAtomicStore

An abstract superclass that you subclass to create a Core Data atomic store.

class NSAtomicStoreCacheNode

A concrete class that you use to represent basic nodes in a Core Data atomic store.

class NSIncrementalStoreNode

A concrete class used to represent basic nodes in a Core Data incremental store.

