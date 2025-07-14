

- Core Data
- NSPersistentStoreCoordinator
-  addPersistentStore(ofType:configurationName:at:options:) Deprecated

Instance Method

# addPersistentStore(ofType:configurationName:at:options:)

Adds a specific type of persistent store at the provided location.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func addPersistentStore(
    ofType storeType: String,
    configurationName configuration: String?,
    at storeURL: URL?,
    options: [AnyHashable : Any]? = nil
) throws -> NSPersistentStore
```

Deprecated

Use addPersistentStore(type:configuration:at:options:) instead.

## Parameters 

`storeType`  

A string constant (such as `NSSQLiteStoreType`) that specifies the store type—see Persistent Store Types for possible values.

`configuration`  

The name of a configuration in the receiver’s managed object model that will be used by the new store. The configuration can be `nil`, in which case no other configurations are allowed.

`storeURL`  

The file location of the persistent store.

`options`  

A dictionary containing key-value pairs that specify whether the store should be read-only, and whether (for an XML store) the XML file should be validated against the DTD before it is read. For key definitions, see Store options and Migration options. This value may be `nil`.

## Return Value

The newly created store or, if an error occurs, `nil`.

## Mentioned in 

Migrating your data model automatically

## See Also

### Related Documentation

func remove(NSPersistentStore) throws

Removes the specified persistent store from the coordinator.

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, withType: String) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

Deprecated

func importStore(withIdentifier: String?, fromExternalRecordsDirectoryAt: URL, to: URL, options: [AnyHashable : Any]?, ofType: String) throws -> NSPersistentStore

Creates and populates a store with the external records found at a given URL.

Deprecated

### Adding or removing a store

func addPersistentStore(type: NSPersistentStore.StoreType, configuration: String?, at: URL, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

func addPersistentStore(with: NSPersistentStoreDescription, completionHandler: (NSPersistentStoreDescription, (any Error)?) -> Void)

Adds a persistent store using the provided description.

func remove(NSPersistentStore) throws

Removes the specified persistent store from the coordinator.

