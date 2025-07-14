

- UIKit
- UIControl
-  allControlEvents 

Instance Property

# allControlEvents

Returns the events for which the control has associated actions.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var allControlEvents: UIControl.Event { get }
```

## Return Value

A bitmask of constants indicating the events for which this control has associated actions. For a list of possible constants, see the UIControl.Event type.

## Discussion

You can use this method to ascertain which control events trigger actions. More than one action method may be called for a given event.

## See Also

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

func actions(forTarget: Any?, forControlEvent: UIControl.Event) -> [String]?

Returns the actions performed on a target object when the specified event occurs.

func enumerateEventHandlers((UIAction?, (Any?, Selector)?, UIControl.Event, inout Bool) -> Void)

