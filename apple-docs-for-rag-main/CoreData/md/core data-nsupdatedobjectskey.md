

- Core Data
-  NSUpdatedObjectsKey 

Global Variable

# NSUpdatedObjectsKey

A key for the set of objects that were updated.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let NSUpdatedObjectsKey: String
```

## See Also

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

