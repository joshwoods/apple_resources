

- UIKit
- UICollectionViewLayoutAttributes
-  center 

Instance Property

# center

The center point of the item.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var center: CGPoint { get set }
```

## Discussion

The center point is specified in the coordinate system of the collection view. Setting the value of this property also updates the origin of the rectangle in the frame property.

## See Also

### Accessing the layout attributes

var frame: CGRect

The frame rectangle of the item.

var bounds: CGRect

The bounds of the item.

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

