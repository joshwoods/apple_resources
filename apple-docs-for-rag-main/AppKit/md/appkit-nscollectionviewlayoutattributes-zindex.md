

- AppKit
- NSCollectionViewLayoutAttributes
-  zIndex 

Instance Property

# zIndex

The element’s position on the z axis.

macOS 10.11+

``` source
@MainActor
var zIndex: Int { get set }
```

## Discussion

Use this property to specify the front-to-back ordering of items during layout. Items with higher index values appear on top of those with lower values. Items with the same value have an undetermined order.

The default value of this property is `0`.

## See Also

### Accessing the Layout Attributes

var frame: NSRect

The frame rectangle of the element.

var size: NSSize

The size of the element.

var alpha: CGFloat

The transparency of the element.

var isHidden: Bool

A Boolean value indicating whether the element is hidden.

