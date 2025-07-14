

- AppKit
- NSScrollView
-  documentView 

Instance Property

# documentView

The view the scroll view scrolls within its content view.

macOS

``` source
@MainActor
var documentView: NSView? { get set }
```

## See Also

### Related Documentation

var documentView: NSView?

The clip view’s document view.

### Managing the Views

var contentView: NSClipView

The scroll view’s content view, the view that clips the document view.

func addFloatingSubview(NSView, for: NSEvent.GestureAxis)

Adds a floating subview to the document view.

