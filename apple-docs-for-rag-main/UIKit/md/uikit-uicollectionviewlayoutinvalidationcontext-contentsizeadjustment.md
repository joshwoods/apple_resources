

- UIKit
- UICollectionViewLayoutInvalidationContext
-  contentSizeAdjustment 

Instance Property

# contentSizeAdjustment

The delta value to be applied to the collection view’s content size.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var contentSizeAdjustment: CGSize { get set }
```

## Discussion

Use this property to update the size of the collection view’s content area. The default value of this property is CGSizeZero. Changing the value causes the collection view to add the specified height and width values to its contentSize property. Thus, positive values grow the content area and negative values shrink it.

## See Also

### Invalidating the Content Area

var contentOffsetAdjustment: CGPoint

The delta value to be applied to the collection view’s content offset.

