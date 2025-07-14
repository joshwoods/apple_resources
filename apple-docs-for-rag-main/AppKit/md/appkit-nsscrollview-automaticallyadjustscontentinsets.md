

- AppKit
- NSScrollView
-  automaticallyAdjustsContentInsets 

Instance Property

# automaticallyAdjustsContentInsets

A Boolean that indicates whether the scroll view automatically adjusts its content insets.

macOS 10.10+

``` source
@MainActor
var automaticallyAdjustsContentInsets: Bool { get set }
```

## Discussion

When the value of this property is true, the scroll view automatically sets its contentInsets property to account for any overlapping title or tool bar. To overlap with the title or tool bar, the window style mask must include `NSFullSizeContentViewWindowMask` and the title bar must not be transparent.

The default value of this property is true.

## See Also

### Managing Insets

var contentInsets: NSEdgeInsets

The distance that the scroll view’s subviews are inset from the enclosing scroll view during tiling.

var scrollerInsets: NSEdgeInsets

The distance the scrollers are inset from the edge of the scroll view.

