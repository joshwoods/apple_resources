

- Core Data
- NSManagedObjectContext
-  obtainPermanentIDs(for:) 

Instance Method

# obtainPermanentIDs(for:)

Converts to permanent IDs the object IDs of the objects in a given array.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func obtainPermanentIDs(for objects: [NSManagedObject]) throws
```

## Parameters 

`objects`  

An array of managed objects.

## Discussion

This method converts the object ID of each managed object in `objects` to a permanent ID. Although the object will have a permanent ID, it will still respond positively to isInserted until it is saved. Any object that already has a permanent ID is ignored.

Any object not already assigned to a store is assigned based on the same rules Core Data uses for assignment during a save operation (first writable store supporting the entity, and appropriate for the instance and its related items).

### Special Considerations

This method results in a transaction with the underlying store which changes the file’s modification date.

In macOS, this results an additional consideration if you invoke this method on the managed object context associated with an instance of NSPersistentDocument. Instances of `NSDocument` need to know that they are in sync with the underlying content. To avoid problems, after invoking this method you must therefore update the document’s modification date (using fileModificationDate).

## See Also

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

func assign(Any, to: NSPersistentStore)

Specifies the store in which a newly inserted object will be saved.

func detectConflicts(for: NSManagedObject)

Marks an object for conflict detection.

func refresh(NSManagedObject, mergeChanges: Bool)

Updates the persistent properties of a managed object to use the latest values from the persistent store.

func processPendingChanges()

Forces the context to process changes to the object graph.

func observeValue(forKeyPath: String?, of: Any?, change: [String : Any]?, context: UnsafeMutableRawPointer?)

Allows a context that has registered as an observer of a value to be notified of a change to that value.

