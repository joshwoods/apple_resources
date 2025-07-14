

- UIKit
- UIControl
-  sendActions(for:) 

Instance Method

# sendActions(for:)

Calls the action methods associated with the specified events.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func sendActions(for controlEvents: UIControl.Event)
```

## Parameters 

`controlEvents`  

A bitmask with flags that specify the control events for which the control sends action messages. See UIControl.Event for bitmask constants.

## Discussion

You call this method when you want the control to perform the actions associated with the specified events. This method iterates over the control’s registered targets and action methods and calls the sendAction(_:to:for:) method for each one that is associated with an event in the `controlEvents` parameter.

## See Also

### Related Documentation

func addTarget(Any?, action: Selector, for: UIControl.Event)

Associates a target object and action method with the control.

### Triggering actions

func performPrimaryAction()

Calls the method associated with the control’s primary action.

func sendAction(UIAction)

func sendAction(Selector, to: Any?, for: UIEvent?)

Calls the specified action method.

