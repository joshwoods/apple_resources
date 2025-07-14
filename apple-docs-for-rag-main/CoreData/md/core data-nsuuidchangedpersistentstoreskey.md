

- Core Data
-  NSUUIDChangedPersistentStoresKey 

Global Variable

# NSUUIDChangedPersistentStoresKey

Key for an array containing the old and new stores.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let NSUUIDChangedPersistentStoresKey: String
```

## Discussion

The object at index `0` is the old store instance, and the object at index `1` the new. When migration happens, the array contains a third object (at index `2`) that is an array containing the new objectIDs for all the migrated objects.

## See Also

### Constants

let NSAddedPersistentStoresKey: String

Key for the array of stores that were added.

let NSRemovedPersistentStoresKey: String

Key for the array of stores that were removed.

let NSPersistentStoreConnectionPoolMaxSizeKey: String

The maximum connection pool size to use on a store that supports concurrent request handling.

let NSPersistentStoreSaveConflictsErrorKey: String

The key for the array of merge conflict objects (instances of NSMergeConflict).

let NSPersistentStoreUbiquitousTransitionTypeKey: StringDeprecated

