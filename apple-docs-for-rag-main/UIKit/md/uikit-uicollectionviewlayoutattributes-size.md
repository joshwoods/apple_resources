

- UIKit
- UICollectionViewLayoutAttributes
-  size 

Instance Property

# size

The size of the item.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var size: CGSize { get set }
```

## Discussion

Setting the value of this property also changes the size of the rectangle returned by the frame and bounds properties.

## See Also

### Accessing the layout attributes

var frame: CGRect

The frame rectangle of the item.

var bounds: CGRect

The bounds of the item.

var center: CGPoint

The center point of the item.

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

