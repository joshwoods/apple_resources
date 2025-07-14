

- RealityKit
- ARView
-  keyUp(with:) 

Instance Method

# keyUp(with:)

Informs the view that the user has released a key.

macOS

``` source
@MainActor @preconcurrency
override dynamic func keyUp(with event: NSEvent)
```

## Parameters 

`event`  

An object encapsulating information about the key-up event.

## Discussion

The view handles the event instead of passing it to the next responder. See NSResponder for more information about the responder chain.

## See Also

### Handling keyboard input

var acceptsFirstResponder: Bool

A Boolean value that indicates whether the view accepts first responder status.

func keyDown(with: NSEvent)

Informs the view that the user has pressed a key.

