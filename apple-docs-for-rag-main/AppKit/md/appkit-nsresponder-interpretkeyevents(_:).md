

- AppKit
- NSResponder
-  interpretKeyEvents(\_:) 

Instance Method

# interpretKeyEvents(\_:)

Handles a series of key events.

macOS

``` source
@MainActor
func interpretKeyEvents(_ eventArray: [NSEvent])
```

## Parameters 

`eventArray`  

An array of key-event characters to give to the system input manager.

## Discussion

This method, which is invoked by subclasses from the keyDown(with:) method, sends the character input in `eventArray` to the system input manager for interpretation as text to insert or commands to perform. The input manager responds to the request by sending insertText(_:) and doCommand(by:) messages back to the invoker of this method. Subclasses shouldn’t override this method.

See the NSInputManager and NSTextInput class and protocol specifications for more information on input management.

## See Also

### Responding to Key Events

func keyDown(with: NSEvent)

Informs the receiver that the user has pressed a key.

func keyUp(with: NSEvent)

Informs the receiver that the user has released a key.

func performKeyEquivalent(with: NSEvent) -> Bool

Handle a key equivalent.

func flushBufferedKeyEvents()

Clears any unprocessed key events when overridden by subclasses.

