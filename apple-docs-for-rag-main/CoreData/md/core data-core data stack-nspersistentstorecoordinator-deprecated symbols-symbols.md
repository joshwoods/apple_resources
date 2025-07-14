

- Core Data
- Core Data stack
- NSPersistentStoreCoordinator
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Deprecated constants

let NSXMLExternalRecordType: String

Specifies an XML file format.

Deprecated

let NSBinaryExternalRecordType: String

Specifies a binary file format

Deprecated

### Deprecated enumerations

enum NSPersistentStoreUbiquitousTransitionType

These constants are used as the value corresponding to the NSPersistentStoreUbiquitousTransitionTypeKey in the user info dictionary of NSPersistentStoreCoordinatorStoresWillChangeNotification and NSPersistentStoreCoordinatorStoresDidChangeNotification notifications to identify the type of event leading to a change.

Deprecated

### Deprecated type properties

static let NSPersistentStoreDidImportUbiquitousContentChanges: NSNotification.Name

Posted after records are imported from the ubiquitous content store.

Deprecated

### Deprecated type methods

class func elementsDerived(fromExternalRecordAt: URL) -> [AnyHashable : Any]

Returns a dictionary containing the parsed elements derived from the Spotlight external record file that is specified by the given URL.

Deprecated

class func metadataForPersistentStore(with: URL) throws -> [AnyHashable : Any]

Returns a dictionary that contains the metadata stored in the persistent store at the specified location.

Deprecated

class func metadataForPersistentStore(ofType: String?, at: URL) throws -> [String : Any]

Returns a dictionary containing the metadata stored in the persistent store at a given URL.

Deprecated

class func metadataForPersistentStore(ofType: String, at: URL, options: [AnyHashable : Any]?) throws -> [String : Any]

Returns the metadata of a specific type of persistent store at the provided location.

Deprecated

class func registerStoreClass(AnyClass?, forStoreType: String)

Registers a persistent store subclass using the specified store type identifier.

Deprecated

class func removeUbiquitousContentAndPersistentStore(at: URL, options: [AnyHashable : Any]?) throws

Deletes all ubiquitous content for all peers for the persistent store at a given URL and also delete the local store file.

Deprecated

class func setMetadata([String : Any]?, forPersistentStoreOfType: String?, at: URL) throws

Sets the metadata for a given store.

Deprecated

class func setMetadata([String : Any]?, forPersistentStoreOfType: String, at: URL, options: [AnyHashable : Any]?) throws

Updates the metadata of a specific type of persistent store at the provided location.

Deprecated

### Deprecated instance methods

func addPersistentStore(ofType: String, configurationName: String?, at: URL?, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

Deprecated

func destroyPersistentStore(at: URL, ofType: String, options: [AnyHashable : Any]?) throws

Deletes a specific type of persistent store at the provided location.

Deprecated

func importStore(withIdentifier: String?, fromExternalRecordsDirectoryAt: URL, to: URL, options: [AnyHashable : Any]?, ofType: String) throws -> NSPersistentStore

Creates and populates a store with the external records found at a given URL.

Deprecated

func lock()

Attempts to acquire a lock.

Deprecated

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, withType: String) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

Deprecated

func replacePersistentStore(at: URL, destinationOptions: [AnyHashable : Any]?, withPersistentStoreFrom: URL, sourceOptions: [AnyHashable : Any]?, ofType: String) throws

Replaces one persistent store with another.

Deprecated

func tryLock() -> Bool

Attempts to acquire a lock.

Deprecated

func unlock()

Relinquishes a previously acquired lock.

Deprecated

func perform(() -> Void)

Executes the provided closure asynchronously on the coordinator’s queue.

Deprecated

func performAndWait(() -> Void)

Executes the provided closure on the coordinator’s queue and waits for it to finish.

Deprecated

