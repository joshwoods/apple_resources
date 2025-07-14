

- Core Data
- NSPersistentStoreCoordinator
-  setMetadata(\_:forPersistentStoreOfType:at:) Deprecated

Type Method

# setMetadata(\_:forPersistentStoreOfType:at:)

Sets the metadata for a given store.

iOS 3.0–9.0DeprecatediPadOS 3.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.11DeprecatedtvOSDeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
class func setMetadata(
    _ metadata: [String : Any]?,
    forPersistentStoreOfType storeType: String?,
    at url: URL
) throws
```

Deprecated

Use -setMetadata:forPersistentStoreOfType:URL:options:error: and pass in an options dictionary matching addPersistentStoreWithType

## Parameters 

`metadata`  

A dictionary containing metadata for the store.

`storeType`  

The type of the store at `url`. If this value is `nil`, Core Data will determine which store class should be used to get or set the store file’s metadata by inspecting the file contents.

`url`  

The location of a persistent store.

## See Also

### Related Documentation

func setMetadata([String : Any]?, for: NSPersistentStore)

Updates the metadata for the specified persistent store.

func metadata(for: NSPersistentStore) -> [String : Any]

Returns the metadata of the specified persistent store.

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

class func removeUbiquitousContentAndPersistentStore(at: URL, options: [AnyHashable : Any]?) throws

Deletes all ubiquitous content for all peers for the persistent store at a given URL and also delete the local store file.

Deprecated

class func setMetadata([String : Any]?, forPersistentStoreOfType: String, at: URL, options: [AnyHashable : Any]?) throws

Updates the metadata of a specific type of persistent store at the provided location.

Deprecated

