

- Foundation
- NSNotification
- NSNotification.Name
-  NSManagedObjectContextDidSaveObjectIDs 

Type Property

# NSManagedObjectContextDidSaveObjectIDs

A notification that posts after a context finishes writing changes.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 3.2+

``` source
static let NSManagedObjectContextDidSaveObjectIDs: NSNotification.Name
```

## Discussion

This notification’s `object` is the saved context. Don’t peform any asynchronous work or block the calling thread. NSManagedObjectContext posts notifications to the same thread that creates it.

The `userInfo` dictionary contains the identifiers of the inserted, updated, deleted, and invalidated managed objects. For the keys to access those objects, see NSManagedObjectContext.NotificationKey. It’s safe to capture the dictionary’s contents.

Use this notification instead of NSManagedObjectContextDidSave if you intend to process the changed managed object on a different thread. It’s safe to pass instances of NSManagedObjectID across thread boundaries.

## See Also

### Core Data

static let NSManagedObjectContextDidSave: NSNotification.Name

A notification that posts after a context finishes writing unsaved changes.

static let NSManagedObjectContextObjectsDidChange: NSNotification.Name

A notification that posts when there are changes to context’s registered managed objects.

static let NSManagedObjectContextWillSave: NSNotification.Name

A notification that posts before a context writes unsaved changes.

static let NSPersistentStoreCoordinatorStoresDidChange: NSNotification.Name

A notification that the coordinator posts after its registered stores change.

static let NSPersistentStoreCoordinatorStoresWillChange: NSNotification.Name

A notification that posts before a coordinator changes its registered stores.

static let NSPersistentStoreCoordinatorWillRemoveStore: NSNotification.Name

A notification that posts before a coordinator removes a store.

static let NSCoreDataCoreSpotlightDelegateIndexDidUpdate: NSNotification.Name

A notification that posts after Spotlight completes an index update.

static let NSManagedObjectContextDidMergeChangesObjectIDs: NSNotification.Name

A notification that posts after a context merges changes from a different notification.

static let NSPersistentStoreRemoteChange: NSNotification.Name

A notification that posts after another process writes to a persistent store.

static let NSPersistentStoreDidImportUbiquitousContentChanges: NSNotification.Name

Posted after records are imported from the ubiquitous content store.

Deprecated

