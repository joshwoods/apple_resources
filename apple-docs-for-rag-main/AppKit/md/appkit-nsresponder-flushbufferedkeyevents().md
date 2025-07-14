

- AppKit
- NSResponder
-  flushBufferedKeyEvents() 

Instance Method

# flushBufferedKeyEvents()

Clears any unprocessed key events when overridden by subclasses.

macOS

``` source
@MainActor
func flushBufferedKeyEvents()
```

## See Also

### Responding to Key Events

func keyDown(with: NSEvent)

Informs the receiver that the user has pressed a key.

func keyUp(with: NSEvent)

Informs the receiver that the user has released a key.

func interpretKeyEvents([NSEvent])

Handles a series of key events.

func performKeyEquivalent(with: NSEvent) -> Bool

Handle a key equivalent.

