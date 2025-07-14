

- AppKit
- NSCell
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

A bit mask containing the conditions for sending the action. The only conditions that are actually checked are associated with the NSLeftMouseDownMask, NSLeftMouseUpMask, NSLeftMouseDraggedMask, and NSPeriodicMask bits.

## Return Value

A bit mask containing the previous settings. This bit mask uses the same values as specified in the `mask` parameter.

## Discussion

You use this method during mouse tracking when the mouse button changes state, the mouse moves, or if the cell is marked to send its action continuously while tracking. Because of this, the only bits checked in `mask` are NSLeftMouseDownMask, NSLeftMouseUpMask, NSLeftMouseDraggedMask, and NSPeriodicMask, which are declared in the NSEvent class reference.

You can use the isContinuous property to turn on the flag corresponding to NSPeriodicMask or NSLeftMouseDraggedMask, whichever is appropriate to the given subclass of `NSCell`.

## See Also

### Managing the Target and Action

var action: Selector?

The action performed by the cell.

var target: AnyObject?

The object that receives the cell’s action messages.

var isContinuous: Bool

A Boolean value indicating whether the cell sends its action message continuously during mouse tracking.

