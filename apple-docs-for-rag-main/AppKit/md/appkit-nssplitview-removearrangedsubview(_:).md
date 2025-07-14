

- AppKit
- NSSplitView
-  removeArrangedSubview(\_:) 

Instance Method

# removeArrangedSubview(\_:)

Removes a view as an arranged split pane.

macOS 10.11+

``` source
@MainActor
func removeArrangedSubview(_ view: NSView)
```

## Discussion

If the value of arrangesAllSubviews is false, calling this method doesn’t remove the view as a subview; it remains in the split view’s subviews array.

If you remove a view as a subview (either by calling removeFromSuperview() or removing it from the split view’s subviews array), the system automatically removes the view as an arranged subview.

## See Also

### Arranging Subviews

var arrangesAllSubviews: Bool

A Boolean value that determines whether the split view arranges all of its subviews as split panes.

var arrangedSubviews: [NSView]

The array of views that the split view arranges as its split panes.

func addArrangedSubview(NSView)

Adds a view as an arranged split pane.

func insertArrangedSubview(NSView, at: Int)

Adds a view as an arranged split pane at the specified index.

