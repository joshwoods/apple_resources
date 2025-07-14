

- Core Data
- NSPersistentStore
-  metadata 

Instance Property

# metadata

The metadata for the persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var metadata: [String : Any]! { get set }
```

## Discussion

The dictionary must include the store type (NSStoreTypeKey) and UUID (NSStoreUUIDKey).

### Special Considerations

Subclasses must override this property to provide storage and persistence for the store metadata.

## See Also

### Managing Store Metadata

class func metadataForPersistentStore(with: URL) throws -> [String : Any]

Returns the metadata from the persistent store at the given URL.

class func setMetadata([String : Any]?, forPersistentStoreAt: URL) throws

Sets the metadata for the store at a given URL.

func loadMetadata() throws

Instructs the persistent store to load its metadata.

