

- Core Data
- NSManagedObjectContext
-  shouldDeleteInaccessibleFaults 

Instance Property

# shouldDeleteInaccessibleFaults

A Boolean value that determines whether the context turns inaccessible faults into deleted objects.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var shouldDeleteInaccessibleFaults: Bool { get set }
```

## Discussion

Use this property to control how the context behaves when it encounters an *inaccessible fault* — an object with no underlying data in the persistent store. For example, you might fetch an object that has a to-many relationship, but then a background context deletes the related objects from the store before you traverse that relationship.

When this property is set to true, the context returns a managed object with the following characteristics:

- The object’s attributes, including scalars, nullable, and mandatory attributes are all set to `nil` or `0`.

- The object’s isDeleted property is set to true, which adds the object to the context’s deletedObjects set.

- The object is exempt from validation rules, including optionality, because the object is nonexistent and the context discards it when you next call save() or reset().

When the context returns an object with these characteristics, your app can continue running and process this object in the same way as any other deleted object.

When this property is set to false, the context throws an exception.

The default value is true.

Note

You can use query generations to pin a context to a stable view of the store’s data and isolate that context from changes that other contexts or processes make. For more information, see Accessing data when the store changes.

## See Also

### Handling managed objects

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

