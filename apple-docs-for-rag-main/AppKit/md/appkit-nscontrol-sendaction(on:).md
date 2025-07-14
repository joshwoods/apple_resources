

- AppKit
- NSControl
-  sendAction(on:) 

Instance Method

# sendAction(on:)

Sets the conditions on which the receiver sends action messages to its target.

macOS

``` source
@MainActor
func sendAction(on mask: NSEvent.EventTypeMask) -> Int
```

## Parameters 

`mask`  

A bit mask containing the conditions for sending the action. The only conditions that are actually checked are associated with the `NSLeftMouseDownMask`, `NSLeftMouseUpMask`, `NSLeftMouseDraggedMask`, and `NSPeriodicMask` bits.

## Return Value

A bit mask containing the previous settings. This bit mask uses the same values as specified in the `mask` parameter.

## Discussion

You use this method during mouse tracking when the mouse button changes state, the mouse moves, or if the cell is marked to send its action continuously while tracking. Because of this, the only bits checked in `mask` are `NSLeftMouseDownMask`, `NSLeftMouseUpMask`, `NSLeftMouseDraggedMask`, and `NSPeriodicMask`, which are declared in the NSEvent class reference.

The default implementation of this method simply invokes the sendAction(on:) method of its associated cell.

## See Also

### Related Documentation

func sendAction(on: NSEvent.EventTypeMask) -> Int

Sets the conditions on which the receiver sends action messages to its target.

### Implementing the Target-Action Mechanism

var action: Selector?

The default action-message selector associated with the control.

var target: AnyObject?

The target object that receives action messages from the cell.

var isContinuous: Bool

A Boolean value indicating whether the receiver’s cell sends its action message continuously to its target during mouse tracking.

func sendAction(Selector?, to: Any?) -> Bool

Causes the specified action to be sent to the target.

