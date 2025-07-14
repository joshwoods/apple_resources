

- Core Data
- NSManagedObjectContext
-  didSaveObjectsNotification 

Type Property

# didSaveObjectsNotification

A notification that posts after a context completes a save.

iOS 3.0+iPadOS 3.0+Mac CatalystmacOS 10.4+tvOS 3.0+visionOSwatchOS 1.0+

``` source
static let didSaveObjectsNotification: Notification.Name
```

## Discussion

Important

Use didSaveObjectIDsNotification instead of this notification.

This notification’s `object` is the saved context. Don’t peform any asynchronous work or block the calling thread. NSManagedObjectContext posts notifications to the same thread that creates it.

The `userInfo` dictionary contains the inserted, updated, and deleted managed objects of the completed save. For the keys to access those objects, see NSManagedObjectContext.NotificationKey. Don’t capture the dictionary’s contents.

To safely use the provided managed objects on the current thread, create a new context and use its mergeChanges(fromContextDidSave:) method to merge in the notification’s changes.

## See Also

### Managing notifications

static let didChangeObjectsNotification: Notification.Name

A notification that posts when a context makes changes to its registered objects.

static let NSManagedObjectContextObjectsDidChange: NSNotification.Name

A notification that posts when there are changes to context’s registered managed objects.

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

