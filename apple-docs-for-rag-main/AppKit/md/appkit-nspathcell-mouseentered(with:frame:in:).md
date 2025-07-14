

- AppKit
- NSPathCell
-  mouseEntered(with:frame:in:) 

Instance Method

# mouseEntered(with:frame:in:)

Displays the cell component over which the mouse is hovering.

macOS 10.5+

``` source
@MainActor
func mouseEntered(
    with event: NSEvent,
    frame: NSRect,
    in view: NSView
)
```

## Parameters 

`event`  

The mouse-entered event.

`frame`  

The frame in which the cell is located.

`view`  

The view in which the cell is located.

## Discussion

The `NSPathCell` object dynamically animates to display the component that the mouse is hovering over using mouse-entered and mouse-exited events. The control should call these methods to correctly display the hovered component to the user. The control can acquire rectangles to track using rect(of:withFrame:in:).

## See Also

### Displaying Hidden Components

func mouseExited(with: NSEvent, frame: NSRect, in: NSView)

Hides the cell component over which the mouse is hovering.

