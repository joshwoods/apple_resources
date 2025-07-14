

- AppKit
- NSCollectionViewLayoutAttributes
-  frame 

Instance Property

# frame

The frame rectangle of the element.

macOS 10.11+

``` source
@MainActor
var frame: NSRect { get set }
```

## Discussion

The frame rectangle is measured in points and specified in the collection view’s coordinate system. Setting the value of this property also updates the value in the size property.

## See Also

### Accessing the Layout Attributes

var size: NSSize

The size of the element.

var alpha: CGFloat

The transparency of the element.

var isHidden: Bool

A Boolean value indicating whether the element is hidden.

var zIndex: Int

The element’s position on the z axis.

