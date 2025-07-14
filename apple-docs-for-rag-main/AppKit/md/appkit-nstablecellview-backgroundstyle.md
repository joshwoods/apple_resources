

- AppKit
- NSTableCellView
-  backgroundStyle 

Instance Property

# backgroundStyle

This property is automatically set by the enclosing row view to let this view know what its background looks like.

macOS 10.7+

``` source
@MainActor
var backgroundStyle: NSView.BackgroundStyle { get set }
```

## Discussion

The property is automatically set by the enclosing NSTableRowView to let this view know what its background looks like. For instance, when the `backgroundStyle` is NSBackgroundStyleDark, the view should use a light text color.

The default implementation automatically forwards calls to all subviews that implement `setBackgroundStyle:` or are an NSControl, which have `NSCell` classes that respond to backgroundStyle.

