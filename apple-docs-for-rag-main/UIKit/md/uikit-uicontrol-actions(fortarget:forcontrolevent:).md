

- UIKit
- UIControl
-  actions(forTarget:forControlEvent:) 

Instance Method

# actions(forTarget:forControlEvent:)

Returns the actions performed on a target object when the specified event occurs.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func actions(
    forTarget target: Any?,
    forControlEvent controlEvent: UIControl.Event
) -> [String]?
```

## Parameters 

`target`  

The target object—that is, an object that has an action method associated with this control. You must pass an explicit object for this method to return a meaningful result. Specifying `nil` always returns `nil`.

`controlEvent`  

A single control event constant representing the event for which you want the list of action methods. For a list of possible constants, see UIControl.Event

## Return Value

An array NSString objects containing the selector names of the corresponding action methods, or `nil` if there are no action methods associated with the specified target object and control event.

## Discussion

Use this method to determine what action methods are called on the specified object in response to a particular control event. You can use the NSSelectorFromString(_:) function to convert the returned strings to valid selectors, as needed.

## See Also

### Related Documentation

func sendAction(Selector, to: Any?, for: UIEvent?)

Calls the specified action method.

func sendActions(for: UIControl.Event)

Calls the action methods associated with the specified events.

### Managing the control’s targets and actions

func addTarget(Any?, action: Selector, for: UIControl.Event)

Associates a target object and action method with the control.

func removeTarget(Any?, action: Selector?, for: UIControl.Event)

Stops the delivery of events to the specified target object.

var allTargets: Set&lt;AnyHashable>

Returns all target objects associated with the control.

func addAction(UIAction, for: UIControl.Event)

func removeAction(UIAction, for: UIControl.Event)

func removeAction(identifiedBy: UIAction.Identifier, for: UIControl.Event)

var allControlEvents: UIControl.Event

Returns the events for which the control has associated actions.

func enumerateEventHandlers((UIAction?, (Any?, Selector)?, UIControl.Event, inout Bool) -> Void)

