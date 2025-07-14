

- AppKit
- NSResponder
-  helpRequested(\_:) 

Instance Method

# helpRequested(\_:)

Displays context-sensitive help for the receiver if help has been registered.

macOS

``` source
@MainActor
func helpRequested(_ eventPtr: NSEvent)
```

## Parameters 

`eventPtr`  

An object encapsulating information about the help-request event.

## Discussion

NSWindow invokes this method automatically when the user clicks for help and help has been registered using setContextHelp(_:for:). Otherwise, `NSWindow` passes the message to the next responder. Subclasses are not required to override this method.

Note

Current hardware does not invoke this method and application code should not call it directly. To provide context-sensitive help, use help tags (tooltips). For more information, see macOS Human Interface Guidelines - Help Tags (Tooltips).

## See Also

### Related Documentation

func showContextHelp(Any?)

Implemented by subclasses to invoke the help system, displaying information relevant to the receiver and its current state.

### Responding to Other Kinds of Events

func cursorUpdate(with: NSEvent)

Informs the receiver that the mouse cursor has moved into a cursor rectangle.

func flagsChanged(with: NSEvent)

Informs the receiver that the user has pressed or released a modifier key (Shift, Control, and so on).

func tabletPoint(with: NSEvent)

Informs the receiver that a tablet-point event has occurred.

func tabletProximity(with: NSEvent)

Informs the receiver that a tablet-proximity event has occurred.

func scrollWheel(with: NSEvent)

Informs the receiver that the mouse’s scroll wheel has moved.

func quickLook(with: NSEvent)

Performs a Quick Look on the content at the location specified by the supplied event.

func changeMode(with: NSEvent)

Informs the responder that performed a double-tap on the side of an Apple Pencil.

