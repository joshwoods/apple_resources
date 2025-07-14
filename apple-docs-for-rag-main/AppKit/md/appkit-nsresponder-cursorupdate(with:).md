

- AppKit
- NSResponder
-  cursorUpdate(with:) 

Instance Method

# cursorUpdate(with:)

Informs the receiver that the mouse cursor has moved into a cursor rectangle.

macOS 10.5+

``` source
@MainActor
func cursorUpdate(with event: NSEvent)
```

## Parameters 

`event`  

An object encapsulating information about the cursor-update event (NSCursorUpdate).

## Discussion

Override this method to set the cursor image. The default implementation uses cursor rectangles, if cursor rectangles are currently valid.  If they are not, it calls `super` to send the message up the responder chain.

If the responder implements this method, but decides not to handle a particular event, it should invoke the superclass implementation of this method.

## See Also

### Responding to Other Kinds of Events

func flagsChanged(with: NSEvent)

Informs the receiver that the user has pressed or released a modifier key (Shift, Control, and so on).

func tabletPoint(with: NSEvent)

Informs the receiver that a tablet-point event has occurred.

func tabletProximity(with: NSEvent)

Informs the receiver that a tablet-proximity event has occurred.

func helpRequested(NSEvent)

Displays context-sensitive help for the receiver if help has been registered.

func scrollWheel(with: NSEvent)

Informs the receiver that the mouse’s scroll wheel has moved.

func quickLook(with: NSEvent)

Performs a Quick Look on the content at the location specified by the supplied event.

func changeMode(with: NSEvent)

Informs the responder that performed a double-tap on the side of an Apple Pencil.

