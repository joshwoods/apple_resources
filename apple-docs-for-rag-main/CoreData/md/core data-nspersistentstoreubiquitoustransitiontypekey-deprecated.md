

- Core Data
-  NSPersistentStoreUbiquitousTransitionTypeKey Deprecated

Global Variable

# NSPersistentStoreUbiquitousTransitionTypeKey

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
let NSPersistentStoreUbiquitousTransitionTypeKey: String
```

Deprecated

Please see the release notes and Core Data documentation.

## Description

In the NSPersistentStoreCoordinatorStoresWillChange and NSPersistentStoreCoordinatorStoresDidChange userInfo dictionaries, this identifies the type of event. The corresponding value is one of the NSPersistentStoreUbiquitousTransitionType enum values as an `NSNumber` object.

## See Also

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

