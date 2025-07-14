

- AppKit
- NSControl
-  target 

Instance Property

# target

The target object that receives action messages from the cell.

macOS

``` source
@MainActor
weak var target: AnyObject? { get set }
```

## Discussion

When the value of this property is `nil`, the application follows the responder chain looking for an object that can respond to the message. See the description of the NSActionCell class for details.

## See Also

### Implementing the Target-Action Mechanism

var action: Selector?

The default action-message selector associated with the control.

var isContinuous: Bool

A Boolean value indicating whether the receiver’s cell sends its action message continuously to its target during mouse tracking.

func sendAction(Selector?, to: Any?) -> Bool

Causes the specified action to be sent to the target.

func sendAction(on: NSEvent.EventTypeMask) -> Int

Sets the conditions on which the receiver sends action messages to its target.

