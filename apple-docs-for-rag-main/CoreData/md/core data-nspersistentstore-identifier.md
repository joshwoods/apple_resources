

- Core Data
- NSPersistentStore
-  identifier 

Instance Property

# identifier

The unique identifier for the persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var identifier: String! { get set }
```

## Discussion

The identifier is used as part of the managed object IDs for each object in the store.

### Special Considerations

`NSPersistentStore` provides a default implementation to provide a globally unique identifier for the store instance.

## See Also

### Related Documentation

var metadata: [String : Any]!

The metadata for the persistent store.

### Managing Store Attributes

var isReadOnly: Bool

A Boolean value that indicates whether the persistent store is read-only.

var url: URL?

The URL for the persistent store.

