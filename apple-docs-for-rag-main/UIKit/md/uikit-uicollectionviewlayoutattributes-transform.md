

- UIKit
- UICollectionViewLayoutAttributes
-  transform 

Instance Property

# transform

The affine transform of the item.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var transform: CGAffineTransform { get set }
```

## Discussion

Assigning a value to this property replaces the value in the transform3D property with a 3D version of the affine transform you specify.

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

var alpha: CGFloat

The transparency of the item.

var zIndex: Int

Specifies the item’s position on the z axis.

var isHidden: Bool

Determines whether the item is currently displayed.

