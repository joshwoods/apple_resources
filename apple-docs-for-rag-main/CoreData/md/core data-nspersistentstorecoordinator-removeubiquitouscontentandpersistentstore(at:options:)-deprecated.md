

- Core Data
- NSPersistentStoreCoordinator
-  removeUbiquitousContentAndPersistentStore(at:options:) Deprecated

Type Method

# removeUbiquitousContentAndPersistentStore(at:options:)

Deletes all ubiquitous content for all peers for the persistent store at a given URL and also delete the local store file.

iOS 5.0–10.0DeprecatediPadOS 5.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func removeUbiquitousContentAndPersistentStore(
    at storeURL: URL,
    options: [AnyHashable : Any]? = nil
) throws
```

Deprecated

Please see the release notes and Core Data documentation.

## Parameters 

`storeURL`  

The URL of the store to delete.

`options`  

A dictionary containing the options normally passed to addPersistentStore(ofType:configurationName:at:options:).

## Discussion

Errors may be returned as a result of file I/O, iCloud network or iCloud account issues.

## See Also

### Deprecated type methods

class func elementsDerived(fromExternalRecordAt: URL) -> [AnyHashable : Any]

Returns a dictionary containing the parsed elements derived from the Spotlight external record file that is specified by the given URL.

Deprecated

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

class func setMetadata([String : Any]?, forPersistentStoreOfType: String?, at: URL) throws

Sets the metadata for a given store.

Deprecated

class func setMetadata([String : Any]?, forPersistentStoreOfType: String, at: URL, options: [AnyHashable : Any]?) throws

Updates the metadata of a specific type of persistent store at the provided location.

Deprecated

