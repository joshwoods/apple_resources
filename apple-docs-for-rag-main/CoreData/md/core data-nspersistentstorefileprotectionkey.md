

- Core Data
-  NSPersistentStoreFileProtectionKey 

Global Variable

# NSPersistentStoreFileProtectionKey

Key to represent the protection class for the persistent store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let NSPersistentStoreFileProtectionKey: String
```

## Discussion

Backward compatibility may preclude some features. The acceptable values are those defined for the protectionKey. The default value is completeUntilFirstUserAuthentication for all applications built on or after iOS v5.0. The default value for all older applications is none.

## See Also

### Constants

let NSReadOnlyPersistentStoreOption: String

A flag that indicates whether a store is treated as read-only or not.

let NSValidateXMLStoreOption: String

A flag that indicates whether an XML file should be validated with the DTD while opening.

let NSPersistentStoreTimeoutOption: String

Options key that specifies the connection timeout for Core Data stores.

let NSSQLitePragmasOption: String

Options key for a dictionary of SQLite pragma settings with pragma values indexed by pragma names as keys.

let NSSQLiteAnalyzeOption: String

Option key to run an analysis of the store data to optimize indices based on statistical information when the store is added to the coordinator.

let NSSQLiteManualVacuumOption: String

Option key to rebuild the store file, forcing a database wide defragmentation when the store is added to the coordinator.

let NSPersistentStoreForceDestroyOption: String

A flag that indicates the coordinator destroys the store file even if the operation might be unsafe, overriding locks, if necessary.

