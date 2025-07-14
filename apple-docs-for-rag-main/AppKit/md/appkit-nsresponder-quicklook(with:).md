

- AppKit
- NSResponder
-  quickLook(with:) 

Instance Method

# quickLook(with:)

Performs a Quick Look on the content at the location specified by the supplied event.

macOS 10.8+

``` source
@MainActor
func quickLook(with event: NSEvent)
```

## Parameters 

`event`  

An event object containing the location of the Quick Look content.

## Discussion

The NSEvent.EventType.quickLook event type supports this method. The only valid properties of an NSEvent.EventType.quickLook event are locationInWindow and modifierFlags. A Quick Look event does not come in through the normal event mechanism; therefore, there is no corresponding event mask for it, nor should you attempt to look for it in a sendEvent(_:) message or with the nextEvent(matching:) methods.

If there are no Quick Look items at the location, call super.

`NSResponder` declares but doesn’t implement this method.

## See Also

### Related Documentation

case quickLook

An event that initiates a Quick Look request.

### Responding to Other Kinds of Events

func cursorUpdate(with: NSEvent)

Informs the receiver that the mouse cursor has moved into a cursor rectangle.

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

func changeMode(with: NSEvent)

Informs the responder that performed a double-tap on the side of an Apple Pencil.

