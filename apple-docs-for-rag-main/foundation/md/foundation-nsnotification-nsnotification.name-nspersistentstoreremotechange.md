

- Foundation
- NSNotification
- NSNotification.Name
-  NSPersistentStoreRemoteChange 

Type Property

# NSPersistentStoreRemoteChange

A notification that posts after another process writes to a persistent store.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
static let NSPersistentStoreRemoteChange: NSNotification.Name
```

## Discussion

This notification’s `object` is the changed store coordinator. The framework posts the notification to a private thread. Move to a known thread before peforming any work.

The `userInfo` dictionary contains the store’s URL, the store’s unique identifier, and the transaction’s history token, which you access with the NSPersistentStoreURLKey, NSStoreUUIDKey, and NSPersistentHistoryTokenKey keys. It’s safe to capture the dictionary’s contents.

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

static let NSManagedObjectContextDidSaveObjectIDs: NSNotification.Name

A notification that posts after a context finishes writing changes.

static let NSPersistentStoreDidImportUbiquitousContentChanges: NSNotification.Name

Posted after records are imported from the ubiquitous content store.

Deprecated

