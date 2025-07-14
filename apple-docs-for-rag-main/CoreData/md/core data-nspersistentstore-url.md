

- Core Data
- NSPersistentStore
-  url 

Instance Property

# url

The URL for the persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var url: URL? { get set }
```

## Discussion

To alter the location of a store, send the persistent store coordinator a setURL(_:for:) message.

## See Also

### Managing Store Attributes

var identifier: String!

The unique identifier for the persistent store.

var isReadOnly: Bool

A Boolean value that indicates whether the persistent store is read-only.

