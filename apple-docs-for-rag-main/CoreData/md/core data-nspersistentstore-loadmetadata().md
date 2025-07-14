

- Core Data
- NSPersistentStore
-  loadMetadata() 

Instance Method

# loadMetadata()

Instructs the persistent store to load its metadata.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func loadMetadata() throws
```

## Discussion

There is no way to return an error if the store is invalid.

## See Also

### Managing Store Metadata

class func metadataForPersistentStore(with: URL) throws -> [String : Any]

Returns the metadata from the persistent store at the given URL.

class func setMetadata([String : Any]?, forPersistentStoreAt: URL) throws

Sets the metadata for the store at a given URL.

var metadata: [String : Any]!

The metadata for the persistent store.

