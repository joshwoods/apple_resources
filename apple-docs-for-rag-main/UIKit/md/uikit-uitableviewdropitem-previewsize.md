

- UIKit
- UITableViewDropItem
-  previewSize 

Instance Property

# previewSize

The size of the drag item’s preview.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var previewSize: CGSize { get }
```

**Required**

## Discussion

You might use this property when configuring animations. If the item doesn’t have an associated preview, this property is set to `CGSizeZero`.

## See Also

### Getting the item information

var sourceIndexPath: IndexPath?

The index path of the item in the table view, if any.

**Required**

