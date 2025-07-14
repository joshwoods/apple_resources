

- AppKit
- NSControl
-  isContinuous 

Instance Property

# isContinuous

A Boolean value indicating whether the receiver’s cell sends its action message continuously to its target during mouse tracking.

macOS

``` source
@MainActor
var isContinuous: Bool { get set }
```

## Discussion

The value of this property is true if the action message is sent continuously; otherwise, false.

## See Also

### Implementing the Target-Action Mechanism

var action: Selector?

The default action-message selector associated with the control.

var target: AnyObject?

The target object that receives action messages from the cell.

func sendAction(Selector?, to: Any?) -> Bool

Causes the specified action to be sent to the target.

func sendAction(on: NSEvent.EventTypeMask) -> Int

Sets the conditions on which the receiver sends action messages to its target.

