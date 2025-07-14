

- Core Data
- NSPersistentStoreCoordinator
-  importStore(withIdentifier:fromExternalRecordsDirectoryAt:to:options:ofType:) Deprecated

Instance Method

# importStore(withIdentifier:fromExternalRecordsDirectoryAt:to:options:ofType:)

Creates and populates a store with the external records found at a given URL.

macOS 10.6–10.13Deprecated

``` source
func importStore(
    withIdentifier storeIdentifier: String?,
    fromExternalRecordsDirectoryAt externalRecordsURL: URL,
    to destinationURL: URL,
    options: [AnyHashable : Any]? = nil,
    ofType storeType: String
) throws -> NSPersistentStore
```

Deprecated

Spotlight integration is deprecated. Use CoreSpotlight integration instead.

## Parameters 

`storeIdentifier`  

The identifier for a store.

If this value is `nil` then the method imports the records for the first store found.

`externalRecordsURL`  

The location of the directory containing external records.

`destinationURL`  

An URL object that specifies the location for the new store.

There should be no existing store at this location, as the store will be created from scratch (appending to an existing store is not allowed).

`options`  

A dictionary containing key-value pairs that specify whether the store should be read-only, and whether (for an XML store) the XML file should be validated against the DTD before it is read. For key definitions, see Store options.

`storeType`  

A string constant (such as `NSSQLiteStoreType`) that specifies the type of the new store—see Persistent Store Types.

## Return Value

An object representing the newly-created store.

## See Also

### Related Documentation

func remove(NSPersistentStore) throws

Removes the specified persistent store from the coordinator.

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, withType: String) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

Deprecated

func addPersistentStore(ofType: String, configurationName: String?, at: URL?, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

Deprecated

### Deprecated instance methods

func addPersistentStore(ofType: String, configurationName: String?, at: URL?, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

Deprecated

func destroyPersistentStore(at: URL, ofType: String, options: [AnyHashable : Any]?) throws

Deletes a specific type of persistent store at the provided location.

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

