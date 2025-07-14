

- AppKit
- NSMatrix
-  mouseDown(with:) 

Instance Method

# mouseDown(with:)

Responds to a mouse-down event.

macOS

``` source
@MainActor
func mouseDown(with event: NSEvent)
```

## Parameters 

`event`  

The mouse-down event.

## Discussion

A mouse-down event in a text cell initiates editing mode. A double click in any cell type except a text cell sends the double-click action of the receiver (if there is one) in addition to the single-click action.

Your code should never invoke this method, but you may override it to implement different mouse tracking than NSMatrix does. The response of the receiver depends on its selection mode, as explained in the class description.

## See Also

### Related Documentation

func sendAction() -> Bool

If the selected cell has both an action and a target, sends its action to its target.

func sendDoubleAction()

Sends the double-click action message to the target of the receiver.

### Handling Event and Action Messages

func acceptsFirstMouse(for: NSEvent?) -> Bool

Returns a Boolean value indicating whether the receiver accepts the first mouse.

var mouseDownFlags: Int

The flags in effect at the mouse-down event that started the current tracking session.

func performKeyEquivalent(with: NSEvent) -> Bool

Looks for a cell that has the given key equivalent and, if found, makes that cell respond as if clicked.

