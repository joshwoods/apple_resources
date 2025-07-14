

- AppKit
- NSControl
-  expansionFrame(withFrame:) 

Instance Method

# expansionFrame(withFrame:)

The frame in which a tool tip can be displayed, if needed.

macOS 10.10+

``` source
@MainActor
func expansionFrame(withFrame contentFrame: NSRect) -> NSRect
```

## Parameters 

`contentFrame`  

The frame of the control.

## Return Value

The frame in which the tool tip should be displayed, or NSZeroRect by default.

## Discussion

This method lets the control return an expansion tool tip frame if `contentFrame` is too small for the entire contents in the view. When the pointer hovers over the text in certain controls, the full contents will be shown in a special floating tool tip view. If the frame is big enough to display the contents, return an empty rect from this method and no expansion tool tip view will be shown. Note that some subclasses, such as NSTextField, return the proper frame when required.

## See Also

### Managing Expansion Tool Tips

func draw(withExpansionFrame: NSRect, in: NSView)

Performs custom expansion tool tip drawing.

var allowsExpansionToolTips: Bool

A Boolean value that indicates whether expansion tool tips are shown when the control is hovered over.

