

- Core Data
- NSPersistentStoreCoordinator
-  setMetadata(\_:for:) 

Instance Method

# setMetadata(\_:for:)

Updates the metadata for the specified persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setMetadata(
    _ metadata: [String : Any]?,
    for store: NSPersistentStore
)
```

## Parameters 

`metadata`  

A dictionary containing metadata for the store.

`store`  

A persistent store.

## Discussion

The store type and UUID (`NSStoreTypeKey` and `NSStoreUUIDKey`) are always added automatically, however `NSStoreUUIDKey` is only added if it is not set manually as part of the dictionary argument.

Important

Setting the metadata for a store does not change the information on disk until the store is actually saved.

## See Also

### Related Documentation

class func setMetadata([String : Any]?, forPersistentStoreOfType: String?, at: URL) throws

Sets the metadata for a given store.

Deprecated

class func metadataForPersistentStore(ofType: String?, at: URL) throws -> [String : Any]

Returns a dictionary containing the metadata stored in the persistent store at a given URL.

Deprecated

### Managing a store’s metadata

class func setMetadata([String : Any]?, type: NSPersistentStore.StoreType, at: URL, options: [AnyHashable : Any]?) throws

Updates the metadata of a specific type of persistent store at the provided location.

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

let NSStoreTypeKey: String

A key that identifies the store type.

let NSStoreUUIDKey: String

A key that provides the store’s UUID.

