

- RealityKit
- ARView
-  acceptsFirstResponder 

Instance Property

# acceptsFirstResponder

A Boolean value that indicates whether the view accepts first responder status.

macOS

``` source
@MainActor @preconcurrency
override dynamic var acceptsFirstResponder: Bool { get }
```

## Discussion

An ARView instance sets this value to `true` by default to indicate that it does accept first responder status. See NSResponder for more information about the responder chain.

## See Also

### Handling keyboard input

func keyDown(with: NSEvent)

Informs the view that the user has pressed a key.

func keyUp(with: NSEvent)

Informs the view that the user has released a key.

