

- AppKit
- NSSplitView
-  insertArrangedSubview(\_:at:) 

Instance Method

# insertArrangedSubview(\_:at:)

Adds a view as an arranged split pane at the specified index.

macOS 10.11+

``` source
@MainActor
func insertArrangedSubview(
    _ view: NSView,
    at index: Int
)
```

## Discussion

If the view is already an arranged view, calling this method moves the view to the specified index in the arrangedSubviews array. This change doesn’t affect the view’s index in the split view’s subviews array.

If the view isn’t a subview of the split view, calling this method adds it to the split view’s subviews array.

## See Also

### Arranging Subviews

var arrangesAllSubviews: Bool

A Boolean value that determines whether the split view arranges all of its subviews as split panes.

var arrangedSubviews: [NSView]

The array of views that the split view arranges as its split panes.

func addArrangedSubview(NSView)

Adds a view as an arranged split pane.

func removeArrangedSubview(NSView)

Removes a view as an arranged split pane.

