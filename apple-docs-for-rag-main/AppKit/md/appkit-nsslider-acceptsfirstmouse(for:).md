

- AppKit
- NSSlider
-  acceptsFirstMouse(for:) 

Instance Method

# acceptsFirstMouse(for:)

Returns a Boolean value indicating whether a mouse-down event both activates the window and starts dragging the slider’s knob.

macOS

``` source
@MainActor
func acceptsFirstMouse(for event: NSEvent?) -> Bool
```

## Parameters 

`event`  

The mouse-down event.

## Return Value

true if the receiver accepts the first mouse-down event; otherwise, false. Returns true by default.

## Discussion

If you want the slider to wait for its own mouse-down event, you must override this method.

