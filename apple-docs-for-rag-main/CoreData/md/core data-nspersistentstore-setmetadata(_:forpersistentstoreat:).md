

- Core Data
- NSPersistentStore
-  setMetadata(\_:forPersistentStoreAt:) 

Type Method

# setMetadata(\_:forPersistentStoreAt:)

Sets the metadata for the store at a given URL.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func setMetadata(
    _ metadata: [String : Any]?,
    forPersistentStoreAt url: URL
) throws
```

## Parameters 

`metadata`  

The metadata for the store at `url`.

`url`  

The location of the store.

## Discussion

Subclasses must override this method to set metadata appropriately.

## See Also

### Managing Store Metadata

class func metadataForPersistentStore(with: URL) throws -> [String : Any]

Returns the metadata from the persistent store at the given URL.

func loadMetadata() throws

Instructs the persistent store to load its metadata.

var metadata: [String : Any]!

The metadata for the persistent store.

