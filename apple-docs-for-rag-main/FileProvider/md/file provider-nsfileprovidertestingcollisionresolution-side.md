

- File Provider
- NSFileProviderTestingCollisionResolution
-  side 

Instance Property

# side

The item’s location.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
var side: NSFileProviderTestingOperationSide { get }
```

**Required**

## Discussion

Most operations are symmetrical. They can affect either items stored locally, or items in the File Provider extension’s remote storage.

## See Also

### Accessing the Operation’s Data

var renamedItem: NSFileProviderItem

A description of the renamed item.

**Required**

