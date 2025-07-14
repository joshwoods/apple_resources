

- AppKit
- NSSplitView
-  dividerColor 

Instance Property

# dividerColor

The color of the dividers that the split view draws between subviews.

macOS 10.5+

``` source
@NSCopying @MainActor
var dividerColor: NSColor { get }
```

## Discussion

The default implementation of this method returns clear when the split view’s dividerStyle is NSSplitView.DividerStyle.thick, or when dividerStyle is NSSplitView.DividerStyle.paneSplitter and the split view is in a textured window. The system draws all other thin dividers with a color that provides appropriate contrast between two white panes.

You can subclass NSSplitView and override this method to change the color of dividers.

## See Also

### Configuring and Drawing Dividers

var dividerStyle: NSSplitView.DividerStyle

The style of divider between views.

enum DividerStyle

Constants that specify the style of the split view’s dividers.

var dividerThickness: CGFloat

The thickness of the dividers for the split view.

func drawDivider(in: NSRect)

Draws a divider between two of the split view’s subviews.

