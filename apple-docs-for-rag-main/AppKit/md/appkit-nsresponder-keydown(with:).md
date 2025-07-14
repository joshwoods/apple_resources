

- AppKit
- NSResponder
-  keyDown(with:) 

Instance Method

# keyDown(with:)

Informs the receiver that the user has pressed a key.

macOS

``` source
@MainActor
func keyDown(with event: NSEvent)
```

## Parameters 

`event`  

An object encapsulating information about the key-down event.

## Discussion

The receiver can interpret `event` itself, or pass it to the system input manager using interpretKeyEvents(_:). The default implementation simply passes this message to the next responder.

## See Also

### Responding to Key Events

func keyUp(with: NSEvent)

Informs the receiver that the user has released a key.

func interpretKeyEvents([NSEvent])

Handles a series of key events.

func performKeyEquivalent(with: NSEvent) -> Bool

Handle a key equivalent.

func flushBufferedKeyEvents()

Clears any unprocessed key events when overridden by subclasses.

