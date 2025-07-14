

- Core Data
- NSPersistentStoreCoordinator
-  destroyPersistentStore(at:ofType:options:) Deprecated

Instance Method

# destroyPersistentStore(at:ofType:options:)

Deletes a specific type of persistent store at the provided location.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func destroyPersistentStore(
    at url: URL,
    ofType storeType: String,
    options: [AnyHashable : Any]? = nil
) throws
```

Deprecated

Use destroyPersistentStore(at:type:options:) instead.

## Parameters 

`url`  

The store’s location.

`storeType`  

The store type. For possible values, see NSPersistentStore.StoreType.

`options`  

A dictionary containing key-value pairs that specify store behavior and characteristics. For more information, see Store options.

## See Also

### Modifying a store

func destroyPersistentStore(at: URL, type: NSPersistentStore.StoreType, options: [AnyHashable : Any]?) throws

Deletes a specific type of persistent store at the provided location.

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, type: NSPersistentStore.StoreType) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

func replacePersistentStore(at: URL, destinationOptions: [AnyHashable : Any]?, withPersistentStoreFrom: URL, sourceOptions: [AnyHashable : Any]?, type: NSPersistentStore.StoreType) throws

Replaces one persistent store with another.

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, withType: String) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

Deprecated

func replacePersistentStore(at: URL, destinationOptions: [AnyHashable : Any]?, withPersistentStoreFrom: URL, sourceOptions: [AnyHashable : Any]?, ofType: String) throws

Replaces one persistent store with another.

Deprecated

