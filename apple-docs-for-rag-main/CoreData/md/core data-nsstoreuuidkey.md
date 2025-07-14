

- Core Data
-  NSStoreUUIDKey 

Global Variable

# NSStoreUUIDKey

A key that provides the store’s UUID.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let NSStoreUUIDKey: String
```

## Discussion

The store UUID is useful to identify stores through URI representations, but it is *not* guaranteed to be unique. The UUID generated for new stores is unique—users can freely copy files and thus the UUID stored inside—so if you track or reference stores explicitly you need to be aware of duplicate UUIDs and potentially override the UUID when a new store is added to the list of known stores in your application.

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

let NSStoreTypeKey: String

A key that identifies the store type.

