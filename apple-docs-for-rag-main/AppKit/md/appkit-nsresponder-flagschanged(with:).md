

- AppKit
- NSResponder
-  flagsChanged(with:) 

Instance Method

# flagsChanged(with:)

Informs the receiver that the user has pressed or released a modifier key (Shift, Control, and so on).

macOS

``` source
@MainActor
func flagsChanged(with event: NSEvent)
```

## Parameters 

`event`  

An object encapsulating information about the modifier-key event.

## Discussion

The default implementation simply passes this message to the next responder.

## See Also

### Responding to Other Kinds of Events

func cursorUpdate(with: NSEvent)

Informs the receiver that the mouse cursor has moved into a cursor rectangle.

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

