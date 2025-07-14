

- UIKit
- UICollectionViewLayoutAttributes
-  bounds 

Instance Property

# bounds

The bounds of the item.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var bounds: CGRect { get set }
```

## Discussion

When setting the bounds, the origin of the bounds rectangle must always be at (0, 0). Changing the bounds rectangle also changes the value in the size property to match the new bounds size.

## See Also

### Accessing the layout attributes

var frame: CGRect

The frame rectangle of the item.

var center: CGPoint

The center point of the item.

var size: CGSize

The size of the item.

var transform3D: CATransform3D

The 3D transform of the item.

var transform: CGAffineTransform

The affine transform of the item.

var alpha: CGFloat

The transparency of the item.

var zIndex: Int

Specifies the item’s position on the z axis.

var isHidden: Bool

Determines whether the item is currently displayed.

