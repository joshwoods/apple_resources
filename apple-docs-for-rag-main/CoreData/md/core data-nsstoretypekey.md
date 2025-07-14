

- Core Data
-  NSStoreTypeKey 

Global Variable

# NSStoreTypeKey

A key that identifies the store type.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let NSStoreTypeKey: String
```

## See Also

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

func setMetadata([String : Any]?, for: NSPersistentStore)

Updates the metadata for the specified persistent store.

let NSStoreUUIDKey: String

A key that provides the store’s UUID.

