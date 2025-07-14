

- AppKit
- NSColorPanel
-  dragColor(\_:with:from:) 

Type Method

# dragColor(\_:with:from:)

Drags a color into a destination view from the specified source view.

macOS

``` source
@MainActor
class func dragColor(
    _ color: NSColor,
    with event: NSEvent,
    from sourceView: NSView
) -> Bool
```

## Parameters 

`color`  

The color to drag.

`event`  

The drag event.

`sourceView`  

The view from which the color was dragged.

## Return Value

true

## Discussion

This method is usually invoked by the `mouseDown:` method of `sourceView`. The dragging mechanism handles all subsequent events.

Because it is a class method, dragColor(_:with:from:) can be invoked whether or not the instance of `NSColorPanel` exists.

## See Also

### Setting Color

var color: NSColor

The color of the receiver.

