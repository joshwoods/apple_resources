

- UIKit
- UIControl
-  allTargets 

Instance Property

# allTargets

Returns all target objects associated with the control.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var allTargets: Set { get }
```

## Return Value

A set of all target objects associated with the control. The returned set may include one or more NSNull objects to indicate actions that are dispatched to the responder chain.

## See Also

### Managing the control’s targets and actions

func addTarget(Any?, action: Selector, for: UIControl.Event)

Associates a target object and action method with the control.

func removeTarget(Any?, action: Selector?, for: UIControl.Event)

Stops the delivery of events to the specified target object.

func addAction(UIAction, for: UIControl.Event)

func removeAction(UIAction, for: UIControl.Event)

func removeAction(identifiedBy: UIAction.Identifier, for: UIControl.Event)

func actions(forTarget: Any?, forControlEvent: UIControl.Event) -> [String]?

Returns the actions performed on a target object when the specified event occurs.

var allControlEvents: UIControl.Event

Returns the events for which the control has associated actions.

func enumerateEventHandlers((UIAction?, (Any?, Selector)?, UIControl.Event, inout Bool) -> Void)

