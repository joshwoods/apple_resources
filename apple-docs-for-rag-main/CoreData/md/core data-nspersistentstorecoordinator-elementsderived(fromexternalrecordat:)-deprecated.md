

- Core Data
- NSPersistentStoreCoordinator
-  elementsDerived(fromExternalRecordAt:) Deprecated

Type Method

# elementsDerived(fromExternalRecordAt:)

Returns a dictionary containing the parsed elements derived from the Spotlight external record file that is specified by the given URL.

macOS 10.6–10.13Deprecated

``` source
class func elementsDerived(fromExternalRecordAt fileURL: URL) -> [AnyHashable : Any]
```

Deprecated

Spotlight integration is deprecated. Use CoreSpotlight integration instead.

## Parameters 

`fileURL`  

A file URL specifying the location of a Spotlight external record file.

## Return Value

A dictionary containing the parsed elements derived from the Spotlight support file specified by `fileURL`.

## Discussion

Dictionary keys and the corresponding values are described in Spotlight record keys.

## See Also

### Deprecated type methods

class func metadataForPersistentStore(with: URL) throws -> [AnyHashable : Any]

Returns a dictionary that contains the metadata stored in the persistent store at the specified location.

Deprecated

class func metadataForPersistentStore(ofType: String?, at: URL) throws -> [String : Any]

Returns a dictionary containing the metadata stored in the persistent store at a given URL.

Deprecated

class func metadataForPersistentStore(ofType: String, at: URL, options: [AnyHashable : Any]?) throws -> [String : Any]

Returns the metadata of a specific type of persistent store at the provided location.

Deprecated

class func registerStoreClass(AnyClass?, forStoreType: String)

Registers a persistent store subclass using the specified store type identifier.

Deprecated

class func removeUbiquitousContentAndPersistentStore(at: URL, options: [AnyHashable : Any]?) throws

Deletes all ubiquitous content for all peers for the persistent store at a given URL and also delete the local store file.

Deprecated

class func setMetadata([String : Any]?, forPersistentStoreOfType: String?, at: URL) throws

Sets the metadata for a given store.

Deprecated

class func setMetadata([String : Any]?, forPersistentStoreOfType: String, at: URL, options: [AnyHashable : Any]?) throws

Updates the metadata of a specific type of persistent store at the provided location.

Deprecated

