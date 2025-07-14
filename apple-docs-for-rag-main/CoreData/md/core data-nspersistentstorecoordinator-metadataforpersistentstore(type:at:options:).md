

- Core Data
- NSPersistentStoreCoordinator
-  metadataForPersistentStore(type:at:options:) 

Type Method

# metadataForPersistentStore(type:at:options:)

Returns the metadata of a specific type of persistent store at the provided location.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
class func metadataForPersistentStore(
    type storeType: NSPersistentStore.StoreType,
    at storeURL: URL,
    options: [AnyHashable : Any]? = nil
) throws -> [String : Any]
```

## Parameters 

`storeType`  

The store type. For possible values, see NSPersistentStore.StoreType.

`storeURL`  

The store’s location.

`options`  

A dictionary containing key-value pairs that specify store behavior and characteristics. For more information, see Store options.

## See Also

### Managing a store’s metadata

class func setMetadata([String : Any]?, type: NSPersistentStore.StoreType, at: URL, options: [AnyHashable : Any]?) throws

Updates the metadata of a specific type of persistent store at the provided location.

class func setMetadata([String : Any]?, forPersistentStoreOfType: String, at: URL, options: [AnyHashable : Any]?) throws

Updates the metadata of a specific type of persistent store at the provided location.

Deprecated

class func metadataForPersistentStore(ofType: String, at: URL, options: [AnyHashable : Any]?) throws -> [String : Any]

Returns the metadata of a specific type of persistent store at the provided location.

Deprecated

func metadata(for: NSPersistentStore) -> [String : Any]

Returns the metadata of the specified persistent store.

func setMetadata([String : Any]?, for: NSPersistentStore)

Updates the metadata for the specified persistent store.

let NSStoreTypeKey: String

A key that identifies the store type.

let NSStoreUUIDKey: String

A key that provides the store’s UUID.

