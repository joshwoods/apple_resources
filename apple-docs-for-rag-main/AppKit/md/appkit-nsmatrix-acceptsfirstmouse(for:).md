

- AppKit
- NSMatrix
-  acceptsFirstMouse(for:) 

Instance Method

# acceptsFirstMouse(for:)

Returns a Boolean value indicating whether the receiver accepts the first mouse.

macOS

``` source
@MainActor
func acceptsFirstMouse(for event: NSEvent?) -> Bool
```

## Parameters 

`event`  

This parameter is ignored.

## Return Value

false if the selection mode of the receiver is `NSListModeMatrix`, true if the receiver is in any other selection mode. The receiver does not accept first mouse in `NSListModeMatrix` to prevent the loss of multiple selections.

## See Also

### Related Documentation

var mode: NSMatrix.Mode

The selection mode of the receiver.

### Handling Event and Action Messages

func mouseDown(with: NSEvent)

Responds to a mouse-down event.

var mouseDownFlags: Int

The flags in effect at the mouse-down event that started the current tracking session.

func performKeyEquivalent(with: NSEvent) -> Bool

Looks for a cell that has the given key equivalent and, if found, makes that cell respond as if clicked.

