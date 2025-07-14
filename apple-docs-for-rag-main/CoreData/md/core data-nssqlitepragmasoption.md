

- Core Data
-  NSSQLitePragmasOption 

Global Variable

# NSSQLitePragmasOption

Options key for a dictionary of SQLite pragma settings with pragma values indexed by pragma names as keys.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let NSSQLitePragmasOption: String
```

## Discussion

All pragma values must be specified as `NSString` objects. The `fullfsync` and `synchronous` pragmas control the tradeoff between write performance (write to disk speed & cache utilization) and durability (data loss/corruption sensitivity to power interruption). For more information on pragma settings, see http://sqlite.org/pragma.html.

## See Also

### Constants

let NSReadOnlyPersistentStoreOption: String

A flag that indicates whether a store is treated as read-only or not.

let NSValidateXMLStoreOption: String

A flag that indicates whether an XML file should be validated with the DTD while opening.

let NSPersistentStoreTimeoutOption: String

Options key that specifies the connection timeout for Core Data stores.

let NSSQLiteAnalyzeOption: String

Option key to run an analysis of the store data to optimize indices based on statistical information when the store is added to the coordinator.

let NSSQLiteManualVacuumOption: String

Option key to rebuild the store file, forcing a database wide defragmentation when the store is added to the coordinator.

let NSPersistentStoreFileProtectionKey: String

Key to represent the protection class for the persistent store.

let NSPersistentStoreForceDestroyOption: String

A flag that indicates the coordinator destroys the store file even if the operation might be unsafe, overriding locks, if necessary.

