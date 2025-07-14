

- AppKit
- NSCollectionViewLayoutInvalidationContext
-  contentSizeAdjustment 

Instance Property

# contentSizeAdjustment

The delta value to add to the collection view’s content size.

macOS 10.11+

``` source
@MainActor
var contentSizeAdjustment: NSSize { get set }
```

## Discussion

Use this property to update the size of the collection view’s content area, as computed by the associated layout object. The default value of this property is NSZeroSize. Changing the value causes the collection view to add the specified height and width values to its content size. Thus, positive values grow the content area and negative values shrink it. You might add space around the content area to provide a visual buffer for your collection view content.

## See Also

### Invalidating the Content Area

var contentOffsetAdjustment: NSPoint

The delta value to add to the collection view’s content offset.

