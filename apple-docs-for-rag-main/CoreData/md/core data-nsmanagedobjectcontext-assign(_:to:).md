

- Core Data
- NSManagedObjectContext
-  assign(\_:to:) 

Instance Method

# assign(\_:to:)

Specifies the store in which a newly inserted object will be saved.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func assign(
    _ object: Any,
    to store: NSPersistentStore
)
```

## Parameters 

`object`  

A managed object.

`store`  

A persistent store.

## Discussion

You can obtain a store from the persistent store coordinator, using for example persistentStore(for:).

### Special Considerations

It is only necessary to use this method if the receiver’s persistent store coordinator manages multiple writable stores that have `object`‘s entity in their configuration. Maintaining configurations in the managed object model can eliminate the need for invoking this method directly in many situations. If the receiver’s persistent store coordinator manages only a single writable store, or if only one store has `object`’s entity in its model, `object` will automatically be assigned to that store.

## See Also

### Related Documentation

var persistentStoreCoordinator: NSPersistentStoreCoordinator?

The persistent store coordinator of the context.

### Handling managed objects

var shouldDeleteInaccessibleFaults: Bool

A Boolean value that determines whether the context turns inaccessible faults into deleted objects.

var insertedObjects: Set&lt;NSManagedObject>

The set of objects that have been inserted into the context but not yet saved in a persistent store.

var updatedObjects: Set&lt;NSManagedObject>

The set of objects registered with the context that have uncommitted changes.

var deletedObjects: Set&lt;NSManagedObject>

The set of objects that will be removed from their persistent store during the next save operation.

func shouldHandleInaccessibleFault(NSManagedObject, for: NSManagedObjectID, triggeredByProperty: NSPropertyDescription?) -> Bool

Creates a log of the inaccessible fault.

func insert(NSManagedObject)

Registers an object to be inserted in the context’s persistent store the next time changes are saved.

func delete(NSManagedObject)

Specifies an object that should be removed from its persistent store when changes are committed.

func obtainPermanentIDs(for: [NSManagedObject]) throws

Converts to permanent IDs the object IDs of the objects in a given array.

func detectConflicts(for: NSManagedObject)

Marks an object for conflict detection.

func refresh(NSManagedObject, mergeChanges: Bool)

Updates the persistent properties of a managed object to use the latest values from the persistent store.

func processPendingChanges()

Forces the context to process changes to the object graph.

func observeValue(forKeyPath: String?, of: Any?, change: [String : Any]?, context: UnsafeMutableRawPointer?)

Allows a context that has registered as an observer of a value to be notified of a change to that value.

