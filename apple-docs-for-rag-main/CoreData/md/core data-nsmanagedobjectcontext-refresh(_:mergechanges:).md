

- Core Data
- NSManagedObjectContext
-  refresh(\_:mergeChanges:) 

Instance Method

# refresh(\_:mergeChanges:)

Updates the persistent properties of a managed object to use the latest values from the persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func refresh(
    _ object: NSManagedObject,
    mergeChanges flag: Bool
)
```

## Parameters 

`object`  

A managed object.

`flag`  

A Boolean value.

If `flag` is false, the context discards pending changes and the managed object becomes a fault. Upon next access, the context reloads the object’s values from the persistent store or last cached state.

If `flag` is true, the context reloads the object’s property values from the store or the cache. Then the context applies local changes over the newly loaded values. Merging the local values into `object` always succeeds, and never results in a merge conflict.

## Discussion

If you call this method before the stalenessInterval expires, the context reloads the data from the cache instead of fetching from the store. If `flag` is true, this method doesn’t affect any transient properties. If `flag` is false, the object disposes the value of transient properties.

You typically use this method to ensure data freshness if multiple managed object contexts share a single persistent store. You can use this method to resolve an optimistic locking failure when attempting to save.

Turning `object` into a fault by setting `flag` to false breaks strong references to related managed objects. You can use this method to release a portion of your object graph if you want to constrain memory usage.

## See Also

### Related Documentation

var stalenessInterval: TimeInterval

The maximum length of time that may have elapsed since the store previously fetched data before fulfilling a fault issues a new fetch.

func reset()

Returns the context to its base state.

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

func obtainPermanentIDs(for: [NSManagedObject]) throws

Converts to permanent IDs the object IDs of the objects in a given array.

func detectConflicts(for: NSManagedObject)

Marks an object for conflict detection.

func processPendingChanges()

Forces the context to process changes to the object graph.

func observeValue(forKeyPath: String?, of: Any?, change: [String : Any]?, context: UnsafeMutableRawPointer?)

Allows a context that has registered as an observer of a value to be notified of a change to that value.

