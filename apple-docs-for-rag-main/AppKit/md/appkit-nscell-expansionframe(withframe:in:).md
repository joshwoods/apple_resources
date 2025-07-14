

- AppKit
- NSCell
-  expansionFrame(withFrame:in:) 

Instance Method

# expansionFrame(withFrame:in:)

Returns the expansion cell frame for the receiver.

macOS 10.5+

``` source
@MainActor
func expansionFrame(
    withFrame cellFrame: NSRect,
    in view: NSView
) -> NSRect
```

## Parameters 

`cellFrame`  

The frame for the receiver.

`view`  

The view in which the receiver will be drawn.

## Return Value

The expansion cell frame for the receiver. If the frame is not too small, return an empty rect (NSZeroRect), and no expansion tool tip view will be shown.

## Discussion

This method allows the cell to return an expansion cell frame if `cellFrame` is too small for the entire contents in the view. When the mouse is hovered over the cell in certain controls, the full cell contents are shown in a special floating tool tip view. By default, `NSCell` returns `NSZeroRect`, while some subclasses (such as `NSTextFieldCell`) will return the proper frame when required.

## See Also

### Managing Expansion Frames

func draw(withExpansionFrame: NSRect, in: NSView)

Instructs the receiver to draw in an expansion frame.

