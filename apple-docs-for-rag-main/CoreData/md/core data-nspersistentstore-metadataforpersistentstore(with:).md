

- Core Data
- NSPersistentStore
-  metadataForPersistentStore(with:) 

Type Method

# metadataForPersistentStore(with:)

Returns the metadata from the persistent store at the given URL.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func metadataForPersistentStore(with url: URL) throws -> [String : Any]
```

## Parameters 

`url`  

The location of the store.

## Return Value

The metadata from the persistent store at `url`. Returns `nil` if there is an error.

## Discussion

Subclasses must override this method.

## See Also

### Managing Store Metadata

class func setMetadata([String : Any]?, forPersistentStoreAt: URL) throws

Sets the metadata for the store at a given URL.

func loadMetadata() throws

Instructs the persistent store to load its metadata.

var metadata: [String : Any]!

The metadata for the persistent store.

