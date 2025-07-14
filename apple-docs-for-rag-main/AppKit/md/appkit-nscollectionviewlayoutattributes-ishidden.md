

- AppKit
- NSCollectionViewLayoutAttributes
-  isHidden 

Instance Property

# isHidden

A Boolean value indicating whether the element is hidden.

macOS 10.11+

``` source
@MainActor
var isHidden: Bool { get set }
```

## Discussion

The default value of this property is false. As an optimization, the collection view might not create the corresponding view when the value of this property is true. Because there might not be a view, hidden elements do not participate in hit testing for the collection view.

## See Also

### Accessing the Layout Attributes

var frame: NSRect

The frame rectangle of the element.

var size: NSSize

The size of the element.

var alpha: CGFloat

The transparency of the element.

var zIndex: Int

The element’s position on the z axis.

