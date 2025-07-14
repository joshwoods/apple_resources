

- Core Data
- NSPersistentStoreCoordinator
-  metadataForPersistentStore(ofType:at:options:) Deprecated

Type Method

# metadataForPersistentStore(ofType:at:options:)

Returns the metadata of a specific type of persistent store at the provided location.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func metadataForPersistentStore(
    ofType storeType: String,
    at url: URL,
    options: [AnyHashable : Any]? = nil
) throws -> [String : Any]
```

Deprecated

Use metadataForPersistentStore(type:at:options:) instead.

## Parameters 

`storeType`  

The type of the store. If `nil`, Core Data automatically attempts to determine the store class to use.

`url`  

The file URL of the store.

`options`  

A dictionary that contains options for the store.

## Return Value

A dictionary that contains, at a minimum, values for the NSStoreTypeKey and NSStoreUUIDKey keys.

## See Also

### Managing a store’s metadata

class func setMetadata([String : Any]?, type: NSPersistentStore.StoreType, at: URL, options: [AnyHashable : Any]?) throws

Updates the metadata of a specific type of persistent store at the provided location.

class func metadataForPersistentStore(type: NSPersistentStore.StoreType, at: URL, options: [AnyHashable : Any]?) throws -> [String : Any]

Returns the metadata of a specific type of persistent store at the provided location.

class func setMetadata([String : Any]?, forPersistentStoreOfType: String, at: URL, options: [AnyHashable : Any]?) throws

Updates the metadata of a specific type of persistent store at the provided location.

Deprecated

func metadata(for: NSPersistentStore) -> [String : Any]

Returns the metadata of the specified persistent store.

func setMetadata([String : Any]?, for: NSPersistentStore)

Updates the metadata for the specified persistent store.

let NSStoreTypeKey: String

A key that identifies the store type.

let NSStoreUUIDKey: String

A key that provides the store’s UUID.

