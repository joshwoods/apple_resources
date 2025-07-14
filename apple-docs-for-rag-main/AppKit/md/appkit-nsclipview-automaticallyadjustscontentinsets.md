

- AppKit
- NSClipView
-  automaticallyAdjustsContentInsets 

Instance Property

# automaticallyAdjustsContentInsets

A Boolean value that indicates if the clip view automatically accounts for other scroll view subviews.

macOS 10.10+

``` source
@MainActor
var automaticallyAdjustsContentInsets: Bool { get set }
```

## Discussion

When the value of this property is true, and the clip view is used as the contentView of an NSScrollView, the clip view automatically accounts for other scroll view subviews, such as rulers and headers. The default value is true.

## See Also

### Accessing the Content Insets

var contentInsets: NSEdgeInsets

The distance that the content view is inset from the enclosing scroll view.

