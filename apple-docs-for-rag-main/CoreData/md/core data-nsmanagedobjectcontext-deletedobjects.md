

- Core Data
- NSManagedObjectContext
-  deletedObjects 

Instance Property

# deletedObjects

The set of objects that will be removed from their persistent store during the next save operation.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var deletedObjects: Set { get }
```

## Discussion

The returned set does not necessarily include all the objects that have been deleted (using delete(_:))—if an object has been inserted and deleted without an intervening save operation, it may not be included in the set.

A managed object context does not post key-value observing notifications when the return value of `deletedObjects` changes. A context does, however, post a NSManagedObjectContextObjectsDidChange notification when a change is made, and a NSManagedObjectContextWillSave notification and a NSManagedObjectContextDidSave notification before and after changes are committed respectively (although again the set of deleted objects given for an NSManagedObjectContextDidSave does not include objects that were inserted and deleted without an intervening save operation—that is, they had never been saved to a persistent store).

## See Also

### Handling managed objects

var shouldDeleteInaccessibleFaults: Bool

A Boolean value that determines whether the context turns inaccessible faults into deleted objects.

var insertedObjects: Set&lt;NSManagedObject>

The set of objects that have been inserted into the context but not yet saved in a persistent store.

var updatedObjects: Set&lt;NSManagedObject>

The set of objects registered with the context that have uncommitted changes.

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

