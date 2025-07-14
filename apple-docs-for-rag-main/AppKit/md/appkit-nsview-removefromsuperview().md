

- AppKit
- NSView
-  removeFromSuperview() 

Instance Method

# removeFromSuperview()

Unlinks the view from its superview and its window, removes it from the responder chain, and invalidates its cursor rectangles.

macOS

``` source
@MainActor
func removeFromSuperview()
```

## Discussion

The view is also released; if you plan to reuse it, be sure to retain it before sending this message and to release it as appropriate when adding it as a subview of another `NSView`.

Calling this method removes any constraints that refer to the view you are removing, or that refer to any view in the subtree of the view you are removing.

Never invoke this method during display.

## See Also

### Adding and Removing Subviews

func addSubview(NSView)

Adds a view to the view’s subviews so it’s displayed above its siblings.

func addSubview(NSView, positioned: NSWindow.OrderingMode, relativeTo: NSView?)

Inserts a view among the view’s subviews so it’s displayed immediately above or below another view.

func removeFromSuperviewWithoutNeedingDisplay()

Unlinks the view from its superview and its window and removes it from the responder chain, but does not invalidate its cursor rectangles to cause redrawing.

func replaceSubview(NSView, with: NSView)

Replaces one of the view’s subviews with another view.

func sortSubviews((NSView, NSView, UnsafeMutableRawPointer?) -> ComparisonResult, context: UnsafeMutableRawPointer?)

Orders the view’s immediate subviews using the specified comparator function.

