

- Core Data
- NSPersistentStoreCoordinator
-  migratePersistentStore(\_:to:options:type:) 

Instance Method

# migratePersistentStore(\_:to:options:type:)

Changes the location and, if necessary, the store type of the specified persistent store.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func migratePersistentStore(
    _ store: NSPersistentStore,
    to storeURL: URL,
    options: [AnyHashable : Any]? = nil,
    type storeType: NSPersistentStore.StoreType
) throws -> NSPersistentStore
```

## Parameters 

`store`  

The peristent store to migrate.

`storeURL`  

The location of the new persistent store.

`options`  

A dictionary containing key-value pairs that specify store behavior and characteristics. For more information, see Store options.

`storeType`  

The new store type. For possible values, see NSPersistentStore.StoreType.

## Discussion

Performance may vary depending on the store types of the old and new stores. Invoking this method removes the specified store from the coordinator.

## See Also

### Modifying a store

func destroyPersistentStore(at: URL, type: NSPersistentStore.StoreType, options: [AnyHashable : Any]?) throws

Deletes a specific type of persistent store at the provided location.

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

