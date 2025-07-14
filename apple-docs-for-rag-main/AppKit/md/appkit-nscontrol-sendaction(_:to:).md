

- AppKit
- NSControl
-  sendAction(\_:to:) 

Instance Method

# sendAction(\_:to:)

Causes the specified action to be sent to the target.

macOS

``` source
@MainActor
func sendAction(
    _ action: Selector?,
    to target: Any?
) -> Bool
```

## Parameters 

`action`  

The selector to invoke on the target. If the selector is `NULL`, no message is sent.

`target`  

The target object to receive the message. If the object is `nil`, the application searches the responder chain for an object capable of handling the message. For more information on dispatching actions, see the class description for NSActionCell.

## Return Value

true if the message was successfully sent; otherwise, false.

## Discussion

This method uses the sendAction(_:to:from:) method of `NSApplication` to invoke the specified method on an object. The receiver is passed as the parameter to the action message. This method is invoked primarily by the trackMouse(with:in:of:untilMouseUp:) method of `NSCell`.

## See Also

### Implementing the Target-Action Mechanism

var action: Selector?

The default action-message selector associated with the control.

var target: AnyObject?

The target object that receives action messages from the cell.

var isContinuous: Bool

A Boolean value indicating whether the receiver’s cell sends its action message continuously to its target during mouse tracking.

func sendAction(on: NSEvent.EventTypeMask) -> Int

Sets the conditions on which the receiver sends action messages to its target.

