

- Core Data
- NSIncrementalStore
-  identifierForNewStore(at:) 

Type Method

# identifierForNewStore(at:)

Returns the identifier for the store at a given URL.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func identifierForNewStore(at storeURL: URL) -> Any
```

## Parameters 

`storeURL`  

The URL of a persistent store.

## Return Value

The identifier for the store at `storeURL`.

## See Also

### Accessing Metadata

func loadMetadata() throws

Loads the metadata for the store.

