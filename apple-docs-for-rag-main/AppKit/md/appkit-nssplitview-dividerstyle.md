

- AppKit
- NSSplitView
-  dividerStyle 

Instance Property

# dividerStyle

The style of divider between views.

macOS 10.5+

``` source
@MainActor
var dividerStyle: NSSplitView.DividerStyle { get set }
```

## Discussion

See NSSplitView.DividerStyle for the possible values.

## See Also

### Configuring and Drawing Dividers

enum DividerStyle

Constants that specify the style of the split view’s dividers.

var dividerColor: NSColor

The color of the dividers that the split view draws between subviews.

var dividerThickness: CGFloat

The thickness of the dividers for the split view.

func drawDivider(in: NSRect)

Draws a divider between two of the split view’s subviews.

