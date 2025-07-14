

- AppKit
- NSScrollView
-  contentInsets 

Instance Property

# contentInsets

The distance that the scroll view’s subviews are inset from the enclosing scroll view during tiling.

macOS 10.10+

``` source
@MainActor
var contentInsets: NSEdgeInsets { get set }
```

## Discussion

When the value of this property is equal to `NSEdgeInsetsZero`, traditional tiling is performed. Rulers, headers, and other subviews are tiled with the contentView frame filling the remaining space. When the value of this property is not equal to `NSEdgeInsetsZero`, the rulers, headers, and other subviews are inset as specified. The contentView is placed underneath these sibling views and is only inset by the scroll view border and non-overlay scrollers.

See NSEdgeInsets for possible values.

When the value of the automaticallyAdjustsContentInsets property is true, any value of this property is overridden during tiling.

## See Also

### Managing Insets

var automaticallyAdjustsContentInsets: Bool

A Boolean that indicates whether the scroll view automatically adjusts its content insets.

var scrollerInsets: NSEdgeInsets

The distance the scrollers are inset from the edge of the scroll view.

