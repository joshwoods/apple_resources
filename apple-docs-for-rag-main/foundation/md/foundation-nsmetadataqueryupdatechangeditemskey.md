

- Foundation
-  NSMetadataQueryUpdateChangedItemsKey 

Global Variable

# NSMetadataQueryUpdateChangedItemsKey

The key for retrieving an array of items that have changed in the query result. By default, this array contains NSMetadataItem objects, representing the query’s results; however, the query’s delegate can substitute these objects with instances of a different class.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSMetadataQueryUpdateChangedItemsKey: String
```

## See Also

### Constants

let NSMetadataQueryUpdateAddedItemsKey: String

The key for retrieving an array of items added to the query result. By default, this array contains NSMetadataItem objects, representing the query’s results; however, the query’s delegate can substitute these objects with instances of a different class.

let NSMetadataQueryUpdateRemovedItemsKey: String

The key for retrieving an array of items removed from the query result. By default, this array contains NSMetadataItem objects, representing the query’s results; however, the query’s delegate can substitute these objects with instances of a different class.

