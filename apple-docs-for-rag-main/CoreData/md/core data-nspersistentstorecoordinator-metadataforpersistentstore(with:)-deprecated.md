

- Core Data
- NSPersistentStoreCoordinator
-  metadataForPersistentStore(with:) Deprecated

Type Method

# metadataForPersistentStore(with:)

Returns a dictionary that contains the metadata stored in the persistent store at the specified location.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1–13.1Deprecated

``` source
class func metadataForPersistentStore(with url: URL) throws -> [AnyHashable : Any]
```

Deprecated

Use metadataForPersistentStore(ofType:at:) instead.

## Parameters 

`url`  

An URL object that specifies the location of a persistent store.

## Return Value

A dictionary containing the metadata for the persistent store at `url`. If no store is found, or there is a problem accessing its contents, returns `nil`. The keys guaranteed to be in this dictionary are `NSStoreTypeKey` and `NSStoreUUIDKey`.

## Discussion

This method allows you to access the metadata in a persistent store without initializing a Core Data stack.

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

