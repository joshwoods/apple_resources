

- AppKit
- NSView
-  replaceSubview(\_:with:) 

Instance Method

# replaceSubview(\_:with:)

Replaces one of the view’s subviews with another view.

macOS

``` source
@MainActor
func replaceSubview(
    _ oldView: NSView,
    with newView: NSView
)
```

## Parameters 

`oldView`  

The view to be replaced by `newView`. May not be `nil`.

`newView`  

The view to replace `oldView`. May not be `nil`.

## Discussion

This method does nothing if `oldView` is not a subview of the view.

Neither `oldView` nor `newView` may be `nil`, and the behavior is undefined if either of these parameters is `nil`.

This method causes `oldView` to be released; if you plan to reuse it, be sure to retain it before sending this message and to release it as appropriate when adding it as a subview of another NSView.

Calling this method also removes any constraints associated with `oldView` and its subtree.

## See Also

### Adding and Removing Subviews

func addSubview(NSView)

Adds a view to the view’s subviews so it’s displayed above its siblings.

func addSubview(NSView, positioned: NSWindow.OrderingMode, relativeTo: NSView?)

Inserts a view among the view’s subviews so it’s displayed immediately above or below another view.

func removeFromSuperview()

Unlinks the view from its superview and its window, removes it from the responder chain, and invalidates its cursor rectangles.

func removeFromSuperviewWithoutNeedingDisplay()

Unlinks the view from its superview and its window and removes it from the responder chain, but does not invalidate its cursor rectangles to cause redrawing.

func sortSubviews((NSView, NSView, UnsafeMutableRawPointer?) -> ComparisonResult, context: UnsafeMutableRawPointer?)

Orders the view’s immediate subviews using the specified comparator function.

