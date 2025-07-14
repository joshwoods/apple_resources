

- AppKit
- NSDraggingSession
-  animatesToStartingPositionsOnCancelOrFail 

Instance Property

# animatesToStartingPositionsOnCancelOrFail

Controls whether the dragging image animates back to its starting point on a cancelled or failed drag.

macOS 10.7+

``` source
var animatesToStartingPositionsOnCancelOrFail: Bool { get set }
```

## Discussion

This property should be set immediately after creating the dragging session.

The default value is true.

## See Also

### Dragging Visual Representation

var draggingFormation: NSDraggingFormation

Controls the dragging formation when the drag is not over the source or a valid destination.

