

- AppKit
- NSControl
-  ignoresMultiClick 

Instance Property

# ignoresMultiClick

A Boolean value indicating whether the receiver ignores multiple clicks made in rapid succession.

macOS

``` source
@MainActor
var ignoresMultiClick: Bool { get set }
```

## Discussion

The value of this property is true if the receiver ignores multiple clicks; otherwise, false.

By default, controls treat double clicks as two distinct clicks, triple clicks as three distinct clicks, and so on. However, if you set this propery to true, additional clicks (within a predetermined interval after the first) occurring after the first click are not processed by the receiver, and are instead passed on to `super`.

## See Also

### Tracking the Mouse

func mouseDown(with: NSEvent)

Informs the receiver that the user has pressed the left mouse button.

