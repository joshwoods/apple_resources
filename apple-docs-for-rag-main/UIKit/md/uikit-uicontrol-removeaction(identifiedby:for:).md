

- UIKit
- UIControl
-  removeAction(identifiedBy:for:) 

Instance Method

# removeAction(identifiedBy:for:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
func removeAction(
    identifiedBy actionIdentifier: UIAction.Identifier,
    for controlEvents: UIControl.Event
)
```

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

func actions(forTarget: Any?, forControlEvent: UIControl.Event) -> [String]?

Returns the actions performed on a target object when the specified event occurs.

var allControlEvents: UIControl.Event

Returns the events for which the control has associated actions.

func enumerateEventHandlers((UIAction?, (Any?, Selector)?, UIControl.Event, inout Bool) -> Void)

