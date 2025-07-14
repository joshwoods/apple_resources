

- UIKit
- UIControl
-  addTarget(\_:action:for:) 

Instance Method

# addTarget(\_:action:for:)

Associates a target object and action method with the control.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addTarget(
    _ target: Any?,
    action: Selector,
    for controlEvents: UIControl.Event
)
```

## Parameters 

`target`  

The target object—that is, the object whose `action` method is called. If you specify `nil`, UIKit searches the responder chain for an object that responds to the specified action message and delivers the message to that object.

`action`  

A selector identifying the action method to be called. You may specify a selector whose signature matches any of the signatures in the code example in UIControl. This parameter must not be `nil`.

`controlEvents`  

A bitmask specifying the control-specific events for which the action method is called. Always specify at least one constant. For a list of possible constants, see UIControl.Event.

## Mentioned in 

Responding to control-based events using target-action

## Discussion

You may call this method multiple times to configure multiple targets and actions for the control. It is also safe to call this method multiple times with the same values for the `target` and `action` parameters. The control maintains a list of its attached targets and actions along with the events each supports.

The control does not retain the object in the `target` parameter. It is your responsibility to maintain a strong reference to the target object while it is attached to a control.

Specifying a value of `0` for the `controlEvents` parameter does not prevent events from being sent to a previously registered `target` and `action` method. To stop the delivery of events, always call the removeTarget(_:action:for:) method.

## See Also

### Managing the control’s targets and actions

func removeTarget(Any?, action: Selector?, for: UIControl.Event)

Stops the delivery of events to the specified target object.

var allTargets: Set&lt;AnyHashable>

Returns all target objects associated with the control.

func addAction(UIAction, for: UIControl.Event)

func removeAction(UIAction, for: UIControl.Event)

func removeAction(identifiedBy: UIAction.Identifier, for: UIControl.Event)

func actions(forTarget: Any?, forControlEvent: UIControl.Event) -> [String]?

Returns the actions performed on a target object when the specified event occurs.

var allControlEvents: UIControl.Event

Returns the events for which the control has associated actions.

func enumerateEventHandlers((UIAction?, (Any?, Selector)?, UIControl.Event, inout Bool) -> Void)

