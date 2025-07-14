

- AppKit
- NSControl
-  draw(withExpansionFrame:in:) 

Instance Method

# draw(withExpansionFrame:in:)

Performs custom expansion tool tip drawing.

macOS 10.10+

``` source
@MainActor
func draw(
    withExpansionFrame contentFrame: NSRect,
    in view: NSView
)
```

## Parameters 

`contentFrame`  

The frame in which to draw.

`view`  

The view in which to draw.

## Discussion

Note that the view may be different from the original view in which the text appeared.

## See Also

### Managing Expansion Tool Tips

var allowsExpansionToolTips: Bool

A Boolean value that indicates whether expansion tool tips are shown when the control is hovered over.

func expansionFrame(withFrame: NSRect) -> NSRect

The frame in which a tool tip can be displayed, if needed.

