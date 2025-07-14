

- AppKit
- NSScrollView
-  contentView 

Instance Property

# contentView

The scroll view’s content view, the view that clips the document view.

macOS

``` source
@MainActor
var contentView: NSClipView { get set }
```

## Discussion

Setting the value of this property to an `NSClipView` that has a document view also sets the scroll view’s document view to be the document view of that `NSClipView`. The original content view retains its document view.

## See Also

### Managing the Views

var documentView: NSView?

The view the scroll view scrolls within its content view.

func addFloatingSubview(NSView, for: NSEvent.GestureAxis)

Adds a floating subview to the document view.

