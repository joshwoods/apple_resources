

- AppKit
- NSPathCell
-  mouseExited(with:frame:in:) 

Instance Method

# mouseExited(with:frame:in:)

Hides the cell component over which the mouse is hovering.

macOS 10.5+

``` source
@MainActor
func mouseExited(
    with event: NSEvent,
    frame: NSRect,
    in view: NSView
)
```

## Parameters 

`event`  

The mouse-exited event.

`frame`  

The frame in which the cell is located.

`view`  

The view in which the cell is located.

## See Also

### Displaying Hidden Components

func mouseEntered(with: NSEvent, frame: NSRect, in: NSView)

Displays the cell component over which the mouse is hovering.

