

- UIKit
- UICollectionViewLayoutInvalidationContext
-  contentOffsetAdjustment 

Instance Property

# contentOffsetAdjustment

The delta value to be applied to the collection view’s content offset.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var contentOffsetAdjustment: CGPoint { get set }
```

## Discussion

Use this property to update the content offset of the collection view. The default value of this property is CGPointZero. Changing the value causes the collection view to add the specified x and y values to its contentOffset property. Thus, positive values increase the content offset and negative values decrease it.

## See Also

### Invalidating the Content Area

var contentSizeAdjustment: CGSize

The delta value to be applied to the collection view’s content size.

