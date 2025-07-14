

- File Provider
- NSFileProviderTestingIngestion
-  item 

Instance Property

# item

A description of the item that changed.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
var item: NSFileProviderItem? { get }
```

**Required**

## Discussion

This property is `nil` for deletion events.

## See Also

### Accessing the Operation’s Data

var itemIdentifier: NSFileProviderItemIdentifier

The unique identifier for the item that changed.

**Required**

var side: NSFileProviderTestingOperationSide

The location where the change occurred.

**Required**

