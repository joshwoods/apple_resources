

- UIKit
- UIControl
-  removeTarget(\_:action:for:) 

Instance Method

# removeTarget(\_:action:for:)

Stops the delivery of events to the specified target object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func removeTarget(
    _ target: Any?,
    action: Selector?,
    for controlEvents: UIControl.Event
)
```

## Parameters 

`target`  

A target object registered with the control. Specify `nil` to remove the specified control events for all target objects.

`action`  

A selector identifying a registered action method. You may specify `nil` for this parameter.

`controlEvents`  

A bitmask specifying the control events that you want to remove for the specified `target` object. For a list of possible constants, see UIControl.Event.

## Discussion

Use this method to prevent the delivery of control events to target objects associated with control. If you specify a valid object in the `target` parameter, this method stops the delivery of the specified events to all action methods associated with that object. If you specify `nil` for the `target` parameter, this method prevents the delivery of those events to all action methods of all target objects.

Although the `action` parameter is not considered when stopping the delivery of events, you should specify an appropriate value anyway. If the specified target/action combination no longer has any valid control events associated with it, the control cleans up its corresponding internal data structures. Doing so can affect the set of objects returned by the allTargets method.

## See Also

### Managing the control’s targets and actions

func addTarget(Any?, action: Selector, for: UIControl.Event)

Associates a target object and action method with the control.

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

