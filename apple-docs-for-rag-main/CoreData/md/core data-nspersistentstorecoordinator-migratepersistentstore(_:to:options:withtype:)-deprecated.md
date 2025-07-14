

- Core Data
- NSPersistentStoreCoordinator
-  migratePersistentStore(\_:to:options:withType:) Deprecated

Instance Method

# migratePersistentStore(\_:to:options:withType:)

Changes the location and, if necessary, the store type of the specified persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func migratePersistentStore(
    _ store: NSPersistentStore,
    to URL: URL,
    options: [AnyHashable : Any]? = nil,
    withType storeType: String
) throws -> NSPersistentStore
```

Deprecated

Use migratePersistentStore(_:to:options:type:) instead.

## Parameters 

`store`  

A persistent store.

`URL`  

An URL object that specifies the location for the new store.

`options`  

A dictionary containing key-value pairs that specify whether the store should be read-only, and whether (for an XML store) the XML file should be validated against the DTD before it is read. For key definitions, see Store options.

`storeType`  

A string constant (such as `NSSQLiteStoreType`) that specifies the type of the new store—see Persistent Store Types.

## Return Value

If the migration is successful, the new store, otherwise `nil`.

## Discussion

This method is typically used for “Save As” operations. Performance may vary depending on the type of old and new store. For more details of the action of this method, see Persistent Store Features in Core Data Programming Guide.

Important

After invocation of this method, the specified store is removed from the coordinator thus `store` is no longer a useful reference.

## See Also

### Related Documentation

func remove(NSPersistentStore) throws

Removes the specified persistent store from the coordinator.

func addPersistentStore(ofType: String, configurationName: String?, at: URL?, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

Deprecated

### Modifying a store

func destroyPersistentStore(at: URL, type: NSPersistentStore.StoreType, options: [AnyHashable : Any]?) throws

Deletes a specific type of persistent store at the provided location.

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, type: NSPersistentStore.StoreType) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

func replacePersistentStore(at: URL, destinationOptions: [AnyHashable : Any]?, withPersistentStoreFrom: URL, sourceOptions: [AnyHashable : Any]?, type: NSPersistentStore.StoreType) throws

Replaces one persistent store with another.

func destroyPersistentStore(at: URL, ofType: String, options: [AnyHashable : Any]?) throws

Deletes a specific type of persistent store at the provided location.

Deprecated

func replacePersistentStore(at: URL, destinationOptions: [AnyHashable : Any]?, withPersistentStoreFrom: URL, sourceOptions: [AnyHashable : Any]?, ofType: String) throws

Replaces one persistent store with another.

Deprecated

