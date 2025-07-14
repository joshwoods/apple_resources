

- AppKit
- NSResponder
-  keyUp(with:) 

Instance Method

# keyUp(with:)

Informs the receiver that the user has released a key.

macOS

``` source
@MainActor
func keyUp(with event: NSEvent)
```

## Parameters 

`event`  

An object encapsulating information about the key-up event.

## Discussion

The default implementation simply passes this message to the next responder.

## See Also

### Responding to Key Events

func keyDown(with: NSEvent)

Informs the receiver that the user has pressed a key.

func interpretKeyEvents([NSEvent])

Handles a series of key events.

func performKeyEquivalent(with: NSEvent) -> Bool

Handle a key equivalent.

func flushBufferedKeyEvents()

Clears any unprocessed key events when overridden by subclasses.

