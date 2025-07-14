

- Core Data
-  NSPersistentStoreConnectionPoolMaxSizeKey 

Global Variable

# NSPersistentStoreConnectionPoolMaxSizeKey

The maximum connection pool size to use on a store that supports concurrent request handling.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
let NSPersistentStoreConnectionPoolMaxSizeKey: String
```

## Discussion

Values that you specify for this key are of type NSNumber. The connection pool size determines the number of requests a store can handle concurrently, and is a function of how many contexts attempt to access store data at any time. Generally, you don’t set this, and use the default value instead.

The default connection pool size is implementation-dependent and may vary by store type or platform.

## See Also

### Constants

let NSAddedPersistentStoresKey: String

Key for the array of stores that were added.

let NSRemovedPersistentStoresKey: String

Key for the array of stores that were removed.

let NSUUIDChangedPersistentStoresKey: String

Key for an array containing the old and new stores.

let NSPersistentStoreSaveConflictsErrorKey: String

The key for the array of merge conflict objects (instances of NSMergeConflict).

let NSPersistentStoreUbiquitousTransitionTypeKey: StringDeprecated

