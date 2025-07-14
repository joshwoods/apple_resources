

- AppKit
- NSCell
-  isContinuous 

Instance Property

# isContinuous

A Boolean value indicating whether the cell sends its action message continuously during mouse tracking.

macOS

``` source
@MainActor
var isContinuous: Bool { get set }
```

## Discussion

When the value of this property is YES, the cell’s action message is sent continuously during mouse tracking. In practice, the continuous delivery of action messages has meaning only for NSActionCell and its subclasses, which implement the target/action mechanism. Some NSControl subclasses, notably NSMatrix, send a default action to a default target when a cell doesn’t provide a target or action.

## See Also

### Managing the Target and Action

var action: Selector?

The action performed by the cell.

var target: AnyObject?

The object that receives the cell’s action messages.

func sendAction(on: NSEvent.EventTypeMask) -> Int

Sets the conditions on which the receiver sends action messages to its target.

