

- AppKit
- NSCollectionViewLayoutAttributes
-  size 

Instance Property

# size

The size of the element.

macOS 10.11+

``` source
@MainActor
var size: NSSize { get set }
```

## Discussion

Setting the value of this property also updates the value in the frame property.

## See Also

### Accessing the Layout Attributes

var frame: NSRect

The frame rectangle of the element.

var alpha: CGFloat

The transparency of the element.

var isHidden: Bool

A Boolean value indicating whether the element is hidden.

var zIndex: Int

The element’s position on the z axis.

