

- Core Data
- NSPersistentStoreCoordinator
-  replacePersistentStore(at:destinationOptions:withPersistentStoreFrom:sourceOptions:ofType:) Deprecated

Instance Method

# replacePersistentStore(at:destinationOptions:withPersistentStoreFrom:sourceOptions:ofType:)

Replaces one persistent store with another.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replacePersistentStore(
    at destinationURL: URL,
    destinationOptions: [AnyHashable : Any]? = nil,
    withPersistentStoreFrom sourceURL: URL,
    sourceOptions: [AnyHashable : Any]? = nil,
    ofType storeType: String
) throws
```

Deprecated

Use replacePersistentStore(at:destinationOptions:withPersistentStoreFrom:sourceOptions:type:) instead.

## Parameters 

`destinationURL`  

The location of the store to replace.

`destinationOptions`  

A dictionary containing key-value pairs that specify the behavior and characteristics of the store to replace. For more information, see Store options.

`sourceURL`  

The location of the store to use as the replacement.

`sourceOptions`  

A dictionary containing key-value pairs that specify the behavior and characteristics of the replacement store. For more information, see Store options.

`storeType`  

The store type of the replacement store. For possible values, see NSPersistentStore.StoreType.

## See Also

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

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, withType: String) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

Deprecated

