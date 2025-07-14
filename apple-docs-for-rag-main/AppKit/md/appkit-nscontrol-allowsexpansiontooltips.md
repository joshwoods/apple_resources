

- AppKit
- NSControl
-  allowsExpansionToolTips 

Instance Property

# allowsExpansionToolTips

A Boolean value that indicates whether expansion tool tips are shown when the control is hovered over.

macOS 10.8+

``` source
@MainActor
var allowsExpansionToolTips: Bool { get set }
```

## Discussion

When the value of this property is true, the expansion tool tip will expand; false means the tool tip won’t expand. The default value is false.

Expansion tooltips are shown when the cell cannot show the full content and the user hovers the pointer over the control. This is controlled by the NSCell class method expansionFrame(withFrame:in:) and is drawn by draw(withExpansionFrame:in:). This value is encoded along with the control.

In general, it is recommended to turn this on for NSTextField instances in a view-based NSTableView.

## See Also

### Managing Expansion Tool Tips

func draw(withExpansionFrame: NSRect, in: NSView)

Performs custom expansion tool tip drawing.

func expansionFrame(withFrame: NSRect) -> NSRect

The frame in which a tool tip can be displayed, if needed.

