

- AppKit
- NSSplitView
-  dividerThickness 

Instance Property

# dividerThickness

The thickness of the dividers for the split view.

macOS

``` source
@MainActor
var dividerThickness: CGFloat { get }
```

## Discussion

You can subclass NSSplitView and override this method to change the thickness of a split view’s dividers.

## See Also

### Configuring and Drawing Dividers

var dividerStyle: NSSplitView.DividerStyle

The style of divider between views.

enum DividerStyle

Constants that specify the style of the split view’s dividers.

var dividerColor: NSColor

The color of the dividers that the split view draws between subviews.

func drawDivider(in: NSRect)

Draws a divider between two of the split view’s subviews.

