

- AppKit
- NSSplitView
-  addArrangedSubview(\_:) 

Instance Method

# addArrangedSubview(\_:)

Adds a view as an arranged split pane.

macOS 10.11+

``` source
@MainActor
func addArrangedSubview(_ view: NSView)
```

## Discussion

If the view isn’t a subview of the split view, calling this method adds it to the split view’s subviews array.

## See Also

### Arranging Subviews

var arrangesAllSubviews: Bool

A Boolean value that determines whether the split view arranges all of its subviews as split panes.

var arrangedSubviews: [NSView]

The array of views that the split view arranges as its split panes.

func insertArrangedSubview(NSView, at: Int)

Adds a view as an arranged split pane at the specified index.

func removeArrangedSubview(NSView)

Removes a view as an arranged split pane.

