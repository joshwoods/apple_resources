

- Core Data
- NSPersistentStoreCoordinator
-  destroyPersistentStore(at:type:options:) 

Instance Method

# destroyPersistentStore(at:type:options:)

Deletes a specific type of persistent store at the provided location.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func destroyPersistentStore(
    at url: URL,
    type storeType: NSPersistentStore.StoreType,
    options: [AnyHashable : Any]? = nil
) throws
```

## Parameters 

`url`  

The store’s location.

`storeType`  

The store type. For possible values, see NSPersistentStore.StoreType.

`options`  

A dictionary containing key-value pairs that specify store behavior and characteristics. For more information, see Store options.

## See Also

### Modifying a store

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, type: NSPersistentStore.StoreType) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

func replacePersistentStore(at: URL, destinationOptions: [AnyHashable : Any]?, withPersistentStoreFrom: URL, sourceOptions: [AnyHashable : Any]?, type: NSPersistentStore.StoreType) throws

Replaces one persistent store with another.

func destroyPersistentStore(at: URL, ofType: String, options: [AnyHashable : Any]?) throws

Deletes a specific type of persistent store at the provided location.

Deprecated

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, withType: String) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

Deprecated

func replacePersistentStore(at: URL, destinationOptions: [AnyHashable : Any]?, withPersistentStoreFrom: URL, sourceOptions: [AnyHashable : Any]?, ofType: String) throws

Replaces one persistent store with another.

Deprecated

