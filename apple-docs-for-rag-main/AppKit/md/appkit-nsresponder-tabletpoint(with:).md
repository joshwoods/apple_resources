

- AppKit
- NSResponder
-  tabletPoint(with:) 

Instance Method

# tabletPoint(with:)

Informs the receiver that a tablet-point event has occurred.

macOS

``` source
@MainActor
func tabletPoint(with event: NSEvent)
```

## Parameters 

`event`  

An object encapsulating information about the tablet-point event.

## Discussion

Tablet events are represented by `NSEvent` objects of type NSTabletPoint. They describe the current state of a transducer (that is, a pointing device) that is in proximity to its tablet, reflecting changes such as location, pressure, tilt, and rotation. See the NSEvent reference for the methods that allow you to extract this and other information from `event`. The default implementation of `NSResponder` passes the message to the next responder.

## See Also

### Responding to Other Kinds of Events

func cursorUpdate(with: NSEvent)

Informs the receiver that the mouse cursor has moved into a cursor rectangle.

func flagsChanged(with: NSEvent)

Informs the receiver that the user has pressed or released a modifier key (Shift, Control, and so on).

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

