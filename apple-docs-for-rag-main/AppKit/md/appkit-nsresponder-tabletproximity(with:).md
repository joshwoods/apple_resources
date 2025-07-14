

- AppKit
- NSResponder
-  tabletProximity(with:) 

Instance Method

# tabletProximity(with:)

Informs the receiver that a tablet-proximity event has occurred.

macOS

``` source
@MainActor
func tabletProximity(with event: NSEvent)
```

## Parameters 

`event`  

An object encapsulating information about the tablet-point event.

## Discussion

Tablet events are represented by `NSEvent` objects of type NSTabletProximity. Tablet devices generate proximity events when the transducer (pointing device) nears a tablet and when it moves away from a tablet. From an event object of this type you can extract information about the kind of device and its capabilities, as well as the relation of this tablet-proximity event to various tablet-point events; see the NSEvent reference for details. The default implementation passes the message to the next responder.

## See Also

### Responding to Other Kinds of Events

func cursorUpdate(with: NSEvent)

Informs the receiver that the mouse cursor has moved into a cursor rectangle.

func flagsChanged(with: NSEvent)

Informs the receiver that the user has pressed or released a modifier key (Shift, Control, and so on).

func tabletPoint(with: NSEvent)

Informs the receiver that a tablet-point event has occurred.

func helpRequested(NSEvent)

Displays context-sensitive help for the receiver if help has been registered.

func scrollWheel(with: NSEvent)

Informs the receiver that the mouse’s scroll wheel has moved.

func quickLook(with: NSEvent)

Performs a Quick Look on the content at the location specified by the supplied event.

func changeMode(with: NSEvent)

Informs the responder that performed a double-tap on the side of an Apple Pencil.

