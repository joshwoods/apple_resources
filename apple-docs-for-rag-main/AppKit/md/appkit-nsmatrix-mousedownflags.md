

- AppKit
- NSMatrix
-  mouseDownFlags 

Instance Property

# mouseDownFlags

The flags in effect at the mouse-down event that started the current tracking session.

macOS

``` source
@MainActor
var mouseDownFlags: Int { get }
```

## Discussion

The NSMatrix mouseDown(with:) method obtains these flags by sending a modifierFlags message to the event passed into mouseDown(with:). Use this property if you want to access these flags. This property is valid only during tracking; it isn’t useful if the target of the receiver initiates another tracking loop as part of its action method (as a cell that pops up a pop-up list does, for example).

## See Also

### Related Documentation

func sendAction(on: NSEvent.EventTypeMask) -> Int

Sets the conditions on which the receiver sends action messages to its target.

### Handling Event and Action Messages

func acceptsFirstMouse(for: NSEvent?) -> Bool

Returns a Boolean value indicating whether the receiver accepts the first mouse.

func mouseDown(with: NSEvent)

Responds to a mouse-down event.

func performKeyEquivalent(with: NSEvent) -> Bool

Looks for a cell that has the given key equivalent and, if found, makes that cell respond as if clicked.

