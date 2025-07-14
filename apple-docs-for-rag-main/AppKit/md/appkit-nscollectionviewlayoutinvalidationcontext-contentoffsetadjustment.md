

- AppKit
- NSCollectionViewLayoutInvalidationContext
-  contentOffsetAdjustment 

Instance Property

# contentOffsetAdjustment

The delta value to add to the collection view’s content offset.

macOS 10.11+

``` source
@MainActor
var contentOffsetAdjustment: NSPoint { get set }
```

## Discussion

The content offset adjustment shifts the position of content inside the collection view by the specified amount. You use this value to make tweaks based on how you want to present your content. For example, you might use it to ensure that the first line of items is always lined up at the same position in the collection view’s visible rectangle. When making adjustments, you can specify both positive and negative values.

The default value of this property is NSZeroSize.

## See Also

### Invalidating the Content Area

var contentSizeAdjustment: NSSize

The delta value to add to the collection view’s content size.

