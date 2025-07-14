

- Foundation
- NSNotification
- NSNotification.Name
-  NSPersistentStoreDidImportUbiquitousContentChanges Deprecated

Type Property

# NSPersistentStoreDidImportUbiquitousContentChanges

Posted after records are imported from the ubiquitous content store.

iOS 5.0–10.0DeprecatediPadOS 5.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static let NSPersistentStoreDidImportUbiquitousContentChanges: NSNotification.Name
```

Deprecated

Please see the release notes and Core Data documentation.

## Discussion

The notification’s `object` is set to the `NSPersistentStoreCoordinator` instance which registered the store. The notification’s `userInfo` dictionary contains the same keys as the NSManagedObjectContextObjectsDidChange notification (NSInsertedObjectsKey, NSUpdatedObjectsKeyNSDeletedObjectsKey), however the values are sets of NSManagedObjectID objects rather than sets of NSManagedObject objects.

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

static let NSPersistentStoreRemoteChange: NSNotification.Name

A notification that posts after another process writes to a persistent store.

