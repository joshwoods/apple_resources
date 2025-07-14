

- AppKit
- NSScrollView
-  addFloatingSubview(\_:for:) 

Instance Method

# addFloatingSubview(\_:for:)

Adds a floating subview to the document view.

macOS 10.9+

``` source
@MainActor
func addFloatingSubview(
    _ view: NSView,
    for axis: NSEvent.GestureAxis
)
```

## Parameters 

`view`  

The view that can float.

`axis`  

The event gesture axis on which the view can float. A view can float on only one axis at a time.

## Discussion

Floating subviews of the document view do not scroll like the rest of the document. Instead these views appear to float over the document. For example, see `NSTableView` floating group rows (floatsGroupRows).

`NSScrollView` ensures that any scrolling on the non-floating axis is performed visually synchronously with the document content.

Note

You are responsible for keeping track of the floating views and removing them via removeFromSuperview() when they should no longer float.

## See Also

### Managing the Views

var contentView: NSClipView

The scroll view’s content view, the view that clips the document view.

var documentView: NSView?

The view the scroll view scrolls within its content view.

