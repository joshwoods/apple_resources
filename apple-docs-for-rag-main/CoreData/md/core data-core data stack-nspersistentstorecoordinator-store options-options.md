

- Core Data
- Core Data stack
- NSPersistentStoreCoordinator
-  Store options 

API Collection

# Store options

The options keys that configure the behavior and characteristics of a persistent store.

## Topics

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

let NSPersistentStoreFileProtectionKey: String

Key to represent the protection class for the persistent store.

let NSPersistentStoreForceDestroyOption: String

A flag that indicates the coordinator destroys the store file even if the operation might be unsafe, overriding locks, if necessary.

### Deprecated

let NSExternalRecordsDirectoryOption: String

Option indicating the directory where Spotlight external record files should be written to.

Deprecated

let NSExternalRecordExtensionOption: String

Option indicating the file extension to use for Spotlight external record files.

Deprecated

let NSExternalRecordsFileFormatOption: String

Option to specify the file format of a Spotlight external records.

Deprecated

let NSPersistentStoreUbiquitousContentNameKey: String

Option to specify that a persistent store has a given name in ubiquity.

Deprecated

let NSPersistentStoreUbiquitousContentURLKey: String

Option to specify the log path to use for ubiquitous content logs.

Deprecated

let NSPersistentStoreUbiquitousPeerTokenOption: String

The corresponding value is an optionally specified string which will be mixed in to Core Data’s identifier for each iCloud peer. The value must be an alphanumeric string without any special characters, whitespace or punctuation. The primary use for this option is to allow multiple applications on the same peer (device) to share a Core Data store integrated with iCloud. Each application will require its own store file.

Deprecated

let NSPersistentStoreRemoveUbiquitousMetadataOption: String

The corresponding value is an `NSNumber` object representing a boolean that indicates whether the receiver should remove all associated ubiquity metadata from a persistent store. You typically use this option during migration or copying to disassociate a persistent store file from an iCloud account.

Deprecated

let NSPersistentStoreUbiquitousContainerIdentifierKey: String

The a string specifying the iCloud container identifier.

Deprecated

let NSPersistentStoreRebuildFromUbiquitousContentOption: String

The corresponding value is an `NSNumber` object representing a boolean that indicates whether the receiver should erase the local store file and rebuild it from the iCloud data in Mobile Documents.

Deprecated

## See Also

### Creating a persistent store coordinator

init(managedObjectModel: NSManagedObjectModel)

Creates a persistent store coordinator with the specified managed object model.

Migration options

The options keys that configure the migration behavior of a persistent store.

Store versions

The metadata keys you use when comparing store versions.

