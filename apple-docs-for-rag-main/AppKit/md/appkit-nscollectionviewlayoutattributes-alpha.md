

- AppKit
- NSCollectionViewLayoutAttributes
-  alpha 

Instance Property

# alpha

The transparency of the element.

macOS 10.11+

``` source
@MainActor
var alpha: CGFloat { get set }
```

## Discussion

Possible values are between `0.0` (fully transparent) and `1.0` (fully opaque). The default value is `1.0`.

Transparent items continue to participate in hit testing for the collection view.

## See Also

### Accessing the Layout Attributes

var frame: NSRect

The frame rectangle of the element.

var size: NSSize

The size of the element.

var isHidden: Bool

A Boolean value indicating whether the element is hidden.

var zIndex: Int

The element’s position on the z axis.

