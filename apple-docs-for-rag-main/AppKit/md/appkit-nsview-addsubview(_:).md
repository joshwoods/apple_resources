

- AppKit
- NSView
-  addSubview(\_:) 

Instance Method

# addSubview(\_:)

Adds a view to the view’s subviews so it’s displayed above its siblings.

macOS

``` source
@MainActor
func addSubview(_ view: NSView)
```

## Parameters 

`view`  

The view to add to the view as a subview.

## Discussion

This method also sets the view as the next responder of `aView`.

The view retains `aView`. If you use removeFromSuperview() to remove `aView` from the view hierarchy, `aView` is released. If you want to keep using `aView` after removing it from the view hierarchy (if, for example, you are swapping through a number of views), you must retain it before invoking removeFromSuperview().

## See Also

### Related Documentation

func viewWillMove(toSuperview: NSView?)

Informs the view that its superview is about to change to the specified superview (which may be `nil`).

var subviews: [NSView]

The array of views embedded in the current view.

func viewWillMove(toWindow: NSWindow?)

Informs the view that it’s being added to the view hierarchy of the specified window object (which may be `nil`).

var nextResponder: NSResponder?

The next responder after this one, or `nil` if it has none.

### Adding and Removing Subviews

func addSubview(NSView, positioned: NSWindow.OrderingMode, relativeTo: NSView?)

Inserts a view among the view’s subviews so it’s displayed immediately above or below another view.

func removeFromSuperview()

Unlinks the view from its superview and its window, removes it from the responder chain, and invalidates its cursor rectangles.

func removeFromSuperviewWithoutNeedingDisplay()

Unlinks the view from its superview and its window and removes it from the responder chain, but does not invalidate its cursor rectangles to cause redrawing.

func replaceSubview(NSView, with: NSView)

Replaces one of the view’s subviews with another view.

func sortSubviews((NSView, NSView, UnsafeMutableRawPointer?) -> ComparisonResult, context: UnsafeMutableRawPointer?)

Orders the view’s immediate subviews using the specified comparator function.

