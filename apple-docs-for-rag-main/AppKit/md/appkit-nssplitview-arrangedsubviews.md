

- AppKit
- NSSplitView
-  arrangedSubviews 

Instance Property

# arrangedSubviews

The array of views that the split view arranges as its split panes.

macOS 10.11+

``` source
@MainActor
var arrangedSubviews: [NSView] { get }
```

## Discussion

This array contains a subset of the views in the split view’s subviews property. The views in this array may appear in a different order than in the subviews array.

If the value of arrangesAllSubviews is true, this array is identical to the subviews array.

## See Also

### Arranging Subviews

var arrangesAllSubviews: Bool

A Boolean value that determines whether the split view arranges all of its subviews as split panes.

func addArrangedSubview(NSView)

Adds a view as an arranged split pane.

func insertArrangedSubview(NSView, at: Int)

Adds a view as an arranged split pane at the specified index.

func removeArrangedSubview(NSView)

Removes a view as an arranged split pane.

