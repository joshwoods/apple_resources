

- AppKit
- NSSplitView
-  drawDivider(in:) 

Instance Method

# drawDivider(in:)

Draws a divider between two of the split view’s subviews.

macOS

``` source
@MainActor
func drawDivider(in rect: NSRect)
```

## Parameters 

`rect`  

The entire divider rectangle in the split view’s flipped coordinate system.

## Discussion

If you override this method to use a custom style for the divider, you may need to change the size of the divider.

## See Also

### Configuring and Drawing Dividers

var dividerStyle: NSSplitView.DividerStyle

The style of divider between views.

enum DividerStyle

Constants that specify the style of the split view’s dividers.

var dividerColor: NSColor

The color of the dividers that the split view draws between subviews.

var dividerThickness: CGFloat

The thickness of the dividers for the split view.

