

- Core Data
- NSIncrementalStore
-  loadMetadata() 

Instance Method

# loadMetadata()

Loads the metadata for the store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func loadMetadata() throws
```

## Discussion

In your implementation of this method, you must validate that the URL used to create the store is usable (the location exists and if necessary is writable, the schema is compatible, and so on) and return an error if there is an issue.

Any subclass of `NSIncrementalStore` which is file-based must be able to handle being initialized with a URL pointing to a zero-length file. This serves as an indicator that a new store is to be constructed at the specified location and allows applications using the store to securely create reservation files in known locations.

## See Also

### Related Documentation

Incremental Store Programming Guide

### Accessing Metadata

class func identifierForNewStore(at: URL) -> Any

Returns the identifier for the store at a given URL.

