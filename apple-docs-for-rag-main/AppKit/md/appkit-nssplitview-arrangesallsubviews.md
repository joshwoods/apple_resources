

- AppKit
- NSSplitView
-  arrangesAllSubviews 

Instance Property

# arrangesAllSubviews

A Boolean value that determines whether the split view arranges all of its subviews as split panes.

macOS 10.11+

``` source
@MainActor
var arrangesAllSubviews: Bool { get set }
```

## Discussion

If the value of this property is true, the split view arranges all of its subviews automatically. The arrangedSubviews array is identical to the split view’s subviews array, so any change to subviews reflects in the arrangedSubviews array. The default value of this property is true.

If the value of this property is false, you must explicitly add a view as an arranged subview to arrange it as a split pane. You add an arranged subview using addArrangedSubview(_:).

When you change the value of this property from true to false, all existing subviews stay as arranged subviews in arrangedSubviews. When you change the value of this property from false to true, all existing subviews become arranged subviews, and the value of the subviews array becomes the arrangedSubviews array.

## See Also

### Arranging Subviews

var arrangedSubviews: [NSView]

The array of views that the split view arranges as its split panes.

func addArrangedSubview(NSView)

Adds a view as an arranged split pane.

func insertArrangedSubview(NSView, at: Int)

Adds a view as an arranged split pane at the specified index.

func removeArrangedSubview(NSView)

Removes a view as an arranged split pane.

