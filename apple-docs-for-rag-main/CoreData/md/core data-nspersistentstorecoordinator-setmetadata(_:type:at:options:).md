

- Core Data
- NSPersistentStoreCoordinator
-  setMetadata(\_:type:at:options:) 

Type Method

# setMetadata(\_:type:at:options:)

Updates the metadata of a specific type of persistent store at the provided location.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
class func setMetadata(
    _ metadata: [String : Any]?,
    type storeType: NSPersistentStore.StoreType,
    at storeURL: URL,
    options: [AnyHashable : Any]? = nil
) throws
```

## Parameters 

`metadata`  

A dictionary that contains the metadata to associate with the store.

`storeType`  

The store type. For possible values, see NSPersistentStore.StoreType.

`storeURL`  

The store’s location.

`options`  

A dictionary containing key-value pairs that specify store behavior and characteristics. For more information, see Store options.

## See Also

### Managing a store’s metadata

class func metadataForPersistentStore(type: NSPersistentStore.StoreType, at: URL, options: [AnyHashable : Any]?) throws -> [String : Any]

Returns the metadata of a specific type of persistent store at the provided location.

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

