

- UIKit
- UICollectionViewLayoutAttributes
-  isHidden 

Instance Property

# isHidden

Determines whether the item is currently displayed.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isHidden: Bool { get set }
```

## Discussion

The default value of this property is false. As an optimization, the collection view might not create the corresponding view if this property is set to true.

## See Also

### Accessing the layout attributes

var frame: CGRect

The frame rectangle of the item.

var bounds: CGRect

The bounds of the item.

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

