

- Core Data
-  NSManagedObjectContext 

Class

# NSManagedObjectContext

An object space to manipulate and track changes to managed objects.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSManagedObjectContext
```

## Mentioned in 

Using Core Data in the background

Setting up a Core Data stack manually

Setting up a Core Data stack

## Overview

A context consists of a group of related model objects that represent an internally consistent view of one or more persistent stores. Changes to managed objects remain in memory in the associated context until Core Data saves that context to one or more persistent stores. A single managed object instance exists in one and only one context, but multiple copies of an object can exist in different contexts. Therefore, an object is unique to a particular context.

### Life cycle management

The context is a powerful object with a central role in the life cycle of managed objects, with responsibilities from life cycle management (including faulting) to validation, inverse relationship handling, and undo/redo. Through a context you can retrieve or “fetch” objects from a persistent store, make changes to those objects, and then either discard the changes or—again through the context—commit them back to the persistent store. The context is responsible for watching for changes in its objects and maintains an undo manager so you can have finer-grained control over undo and redo. You can insert new objects and delete ones you have fetched, and commit these modifications to the persistent store.

All objects fetched from an external store are registered in a context together with a global identifier (an instance of `NSManagedObjectID`) that’s used to uniquely identify each object to the external store.

### Parent store

Managed object contexts have a parent store from which they retrieve data representing managed objects and through which they commit changes to managed objects.

Prior to OS X v10.7 and iOS v5.0, the parent store is always a persistent store coordinator. In macOS 10.7 and later and iOS v5.0 and later, the parent store may be another managed object context. Ultimately the root of a context’s ancestry must be a persistent store coordinator. The coordinator provides the managed object model and dispatches requests to the various persistent stores containing the data.

If a context’s parent store is another managed object context, fetch and save operations are mediated by the parent context instead of a coordinator. This pattern has a number of usage scenarios, including:

- Performing background operations on a second thread or queue.

- Managing discardable edits, such as in an inspector window or view.

As the first scenario implies, a parent context can service requests from children on different threads. You cannot, therefore, use parent contexts created with the thread confinement type (see Concurrency).

When you save changes in a context, the changes are only committed “one store up.” If you save a child context, changes are pushed to its parent. Changes are not saved to the persistent store until the root context is saved. (A root managed object context is one whose parent context is `nil`.) In addition, a parent does not pull changes from children before it saves. You must save a child context if you want ultimately to commit the changes.

### Notifications

A context posts notifications at various points—see NSManagedObjectContextObjectsDidChange for example. Typically, you should register to receive these notifications only from known contexts:

- Swift
- Objective-C

```
NotificationCenter.default.addObserver(self,
                                       selector: #selector(),
                                       name: .NSManagedObjectContextDidSave,
                                       object: )
```

```
[[NSNotificationCenter defaultCenter] addObserver:self
                                      selector:@selector()
                                      name:NSManagedObjectContextDidSaveNotification
                                      object:];
```

Several system frameworks use Core Data internally. If you register to receive these notifications from all contexts (by passing `nil` as the object parameter to a method such as addObserver(_:selector:name:object:)), then you may receive unexpected notifications that are difficult to handle.

### Concurrency

Core Data uses thread (or serialized queue) confinement to protect managed objects and managed object contexts (see Core Data Programming Guide). A consequence of this is that a context assumes the default owner is the thread or queue that creates it. Don’t, therefore, initialize a context on one thread then pass it to another. Instead, pass a reference to a persistent store coordinator and have the receiving thread or queue create a new context using that. If you use Operation, you must create the context in main() (for a serial queue) or start() (for a concurrent queue).

When you create a context you specify the concurrency type with which you’ll use it. When you create a managed object context, you have two options for its thread (queue) association:

- Private: The context creates and manages a private queue.

- Main: The context associates with the main queue and is dependent on the application’s event loop; otherwise, it’s similar to a private context. Use this type for contexts that update view controllers and other user interface elements.

You use contexts using the queue-based concurrency types in conjunction with perform(_:) and performAndWait(_:). You group “standard” messages to send to the context within a block to pass to one of these methods. There are two exceptions:

- Setter methods on queue-based managed object contexts are thread-safe. You can invoke these methods directly on any thread.

- If your code executes on the main thread, you can invoke methods on the main queue style contexts directly instead of using the block based API.

perform(_:) and performAndWait(_:) ensure the block operations execute on the correct queue for the context. The perform(_:) method returns immediately and the context executes the block methods on its own thread. With the performAndWait(_:) method, the context still executes the block methods on its own thread, but the method doesn’t return until the block completes.

It’s important to appreciate that blocks execute as a distinct body of work. As soon as your block ends, anyone else can enqueue another block, undo changes, reset the context, and so on. Thus blocks may be quite large, and typically end by invoking save().

- Swift
- Objective-C

```
var savedOK = false
managedObjectContext.performAndWait() {

    // Perform operations with the context.

    do {
        try managedObjectContext.save()
        savedOK = true
    } catch {
        print("Error saving context: \(error)")
    }
}
```

```
__block BOOL savedOK = NO;
[managedObjectContext performBlockAndWait:^{

    // Perform operations with the context.

    NSError *error = nil;
    if ([managedObjectContext save:&error]) {
        savedOK = YES;
    } else {
        NSLog(@"Error saving: %@", error);
    }
}];
```

You can also perform other operations, such as:

- Swift
- Objective-C

```
let fetchRequest: NSFetchRequest = NSFetchRequest(entityName: "Entity")
var count = 0

managedObjectContext.performAndWait() {
    do {
        count = try managedObjectContext.count(for: fetchRequest)
    } catch {
        print("Error counting objects: \(error)")
    }
}

print("The fetch request would return \(count) objects")
```

```
NSFetchRequest *fetchRequest = [NSFetchRequest fetchRequestWithEntityName:@"Entity"];
__block NSUInteger count = 0;

[managedObjectContext performBlockAndWait:^() {
    NSError *error;
    count = [managedObjectContext countForFetchRequest:fetchRequest error:&error];
    if (count == NSNotFound) {
        NSLog(@"Error counting objects: %@", error);
    }
}];

NSLog(@"The fetch request would return %lu objects", count);
```

### Subclassing notes

You are strongly discouraged from subclassing `NSManagedObjectContext`. The change tracking and undo management mechanisms are highly optimized and hence intricate and delicate. Interposing your own additional logic that might impact processPendingChanges() can have unforeseen consequences. In situations such as store migration, Core Data will create instances of `NSManagedObjectContext` for its own use. Under these circumstances, you cannot rely on any features of your custom subclass. Any `NSManagedObject` subclass must always be fully compatible with `NSManagedObjectContext` (that is, it cannot rely on features of a subclass of `NSManagedObjectContext`).

## Topics

### Creating a context

convenience init(NSManagedObjectContext.ConcurrencyType)

Creates a context that uses the specified concurrency type.

struct ConcurrencyType

The concurrency types to use with a managed object context.

init(concurrencyType: NSManagedObjectContextConcurrencyType)

Creates a context that uses the specified concurrency type.

Deprecated

enum NSManagedObjectContextConcurrencyType

The concurrency types you can use with a managed object context.

### Configuring a context

var persistentStoreCoordinator: NSPersistentStoreCoordinator?

The persistent store coordinator of the context.

var parent: NSManagedObjectContext?

The parent of the context.

var name: String?

The developer-provided name of the context.

var userInfo: NSMutableDictionary

The user information for the context.

### Registering and fetching objects

func fetch(NSFetchRequest&lt;any NSFetchRequestResult>) throws -> [Any]

Returns an array of objects that meet the criteria of the specified fetch request.

func fetch&lt;T>(NSFetchRequest&lt;T>) throws -> [T]

Returns an array of items of the specified type that meet the fetch request’s critieria.

func count(for: NSFetchRequest&lt;any NSFetchRequestResult>) throws -> Int

Returns the number of objects the specified request fetches when it executes.

func registeredObject(for: NSManagedObjectID) -> NSManagedObject?

Returns an object that exists in the context.

func object(with: NSManagedObjectID) -> NSManagedObject

Returns either an existing object from the context or a fault that represents that object.

func existingObject(with: NSManagedObjectID) throws -> NSManagedObject

Returns an existing object from either the context or the persistent store.

var registeredObjects: Set&lt;NSManagedObject>

The set of registered managed objects in the context.

func count&lt;T>(for: NSFetchRequest&lt;T>) throws -> Int

Returns a count of the objects the specified request fetches when it executes.

func execute(NSPersistentStoreRequest) throws -> NSPersistentStoreResult

Passes a request to the persistent store without affecting the contents of the managed object context, and returns a persistent store result.

func refreshAllObjects()

Refreshes all of the registered managed objects in the context.

var retainsRegisteredObjects: Bool

A Boolean value that indicates whether the context keeps strong references to all registered managed objects.

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

func refresh(NSManagedObject, mergeChanges: Bool)

Updates the persistent properties of a managed object to use the latest values from the persistent store.

func processPendingChanges()

Forces the context to process changes to the object graph.

func observeValue(forKeyPath: String?, of: Any?, change: [String : Any]?, context: UnsafeMutableRawPointer?)

Allows a context that has registered as an observer of a value to be notified of a change to that value.

### Managing concurrency

let NSManagedObjectContextQueryGenerationKey: String

Constant used to reference the query generation token.

class func mergeChanges(fromRemoteContextSave: [AnyHashable : Any], into: [NSManagedObjectContext])

Handles changes from other processes or from a serialized state.

var automaticallyMergesChangesFromParent: Bool

A Boolean value that indicates whether the context automatically merges changes saved to its persistent store coordinator or parent context.

var concurrencyType: NSManagedObjectContextConcurrencyType

The concurrency type for the context.

var mergePolicy: Any

The merge policy of the context.

var queryGenerationToken: NSQueryGenerationToken?

Returns the token associated with the query generation currently in use by this context.

var transactionAuthor: String?

The author for the context that is used as an identifier in persistent history transactions.

func mergeChanges(fromContextDidSave: Notification)

Merges the changes specified in a given notification.

func setQueryGenerationFrom(NSQueryGenerationToken?) throws

Sets the query generation this context should use.

### Managing notifications

static let didChangeObjectsNotification: Notification.Name

A notification that posts when a context makes changes to its registered objects.

static let NSManagedObjectContextObjectsDidChange: NSNotification.Name

A notification that posts when there are changes to context’s registered managed objects.

static let didSaveObjectsNotification: Notification.Name

A notification that posts after a context completes a save.

static let NSManagedObjectContextDidSave: NSNotification.Name

A notification that posts after a context finishes writing unsaved changes.

static let willSaveObjectsNotification: Notification.Name

A notification that posts before a context writes pending changes to disk.

static let NSManagedObjectContextWillSave: NSNotification.Name

A notification that posts before a context writes unsaved changes.

let NSInsertedObjectsKey: String

A key for the set of objects that were inserted into the context.

let NSUpdatedObjectsKey: String

A key for the set of objects that were updated.

let NSDeletedObjectsKey: String

A key for the set of objects that were marked for deletion during the previous event.

let NSRefreshedObjectsKey: String

A key for the set of objects that were refreshed but were not dirtied in the scope of this context.

let NSInvalidatedObjectsKey: String

A key for the set of objects that were invalidated.

let NSInvalidatedAllObjectsKey: String

A key that specifies that all objects in the context have been invalidated.

static let didMergeChangesObjectIDsNotification: Notification.Name

A notification that posts after a context finishes merging changes from another notification.

static let didSaveObjectIDsNotification: Notification.Name

A notification that posts after a context finishes saving changes to its managed objects.

enum NotificationKey

Keys to access details in user info dictionaries of managed object context notifications.

### Managing unsaved and uncommitted changes

func save() throws

Attempts to commit unsaved changes to registered objects to the context’s parent store.

var hasChanges: Bool

A Boolean value that indicates whether the context has uncommitted changes.

### Undoing changes

var undoManager: UndoManager?

The object that provides undo support for the context.

func undo()

Sends an undo message to the context’s undo manager, asking it to reverse the latest uncommitted changes applied to objects in the object graph.

func redo()

Sends a redo message to the context’s undo manager, asking it to reverse the latest undo operation applied to objects in the object graph.

func reset()

Returns the context to its base state.

func rollback()

Removes everything from the undo stack, discards all insertions and deletions, and restores updated objects to their last committed values.

### Handling delete propagation

var propagatesDeletesAtEndOfEvent: Bool

A Boolean value that indicates whether the context propagates deletes at the end of the event in which a change was made.

### Managing the staleness interval

var stalenessInterval: TimeInterval

The maximum length of time that may have elapsed since the store previously fetched data before fulfilling a fault issues a new fetch.

### Performing block operations

func perform(() -> Void)

Asynchronously performs the specified closure on the context’s queue.

func perform&lt;T>(schedule: NSManagedObjectContext.ScheduledTaskType, () throws -> T) async rethrows -> T

Submits a closure to the context’s queue for asynchronous execution.

func performAndWait(() -> Void)

Synchronously performs the specified closure on the context’s queue.

func performAndWait&lt;T>(() throws -> T) rethrows -> T

Submits a closure to the context’s queue for synchronous execution.

enum ScheduledTaskType

The different types of scheduled tasks.

### Deprecated

Deprecated symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSEditorRegistration
- NSLocking
- NSObjectProtocol

## See Also

### Object Management

class NSManagedObject

The base class that all Core Data model objects inherit from.

class NSManagedObjectID

A compact, universal identifier for a managed object.

