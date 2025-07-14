

- Core Data
- Core Data stack
- NSPersistentStoreCoordinator
-  Notification keys 

API Collection

# Notification keys

The keys you use to retrieve values from a notification’s user info dictionary.

## Topics

### Constants

let NSAddedPersistentStoresKey: String

Key for the array of stores that were added.

let NSRemovedPersistentStoresKey: String

Key for the array of stores that were removed.

let NSUUIDChangedPersistentStoresKey: String

Key for an array containing the old and new stores.

let NSPersistentStoreConnectionPoolMaxSizeKey: String

The maximum connection pool size to use on a store that supports concurrent request handling.

let NSPersistentStoreSaveConflictsErrorKey: String

The key for the array of merge conflict objects (instances of NSMergeConflict).

let NSPersistentStoreUbiquitousTransitionTypeKey: StringDeprecated

## See Also

### Responding to changes of the coordinator’s registered stores

static let NSPersistentStoreCoordinatorStoresWillChange: NSNotification.Name

A notification that posts before a coordinator changes its registered stores.

static let NSPersistentStoreCoordinatorStoresDidChange: NSNotification.Name

A notification that the coordinator posts after its registered stores change.

static let NSPersistentStoreCoordinatorWillRemoveStore: NSNotification.Name

A notification that posts before a coordinator removes a store.

