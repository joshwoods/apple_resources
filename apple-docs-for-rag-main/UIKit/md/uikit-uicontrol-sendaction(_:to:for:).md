

- UIKit
- UIControl
-  sendAction(\_:to:for:) 

Instance Method

# sendAction(\_:to:for:)

Calls the specified action method.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func sendAction(
    _ action: Selector,
    to target: Any?,
    for event: UIEvent?
)
```

## Parameters 

`action`  

A selector identifying the action method to call. This parameter must not be `nil`.

`target`  

The target object — that is, the object that implements the specified action. Specify nil if you want the app to search the responder chain for an object capable of performing the action.

`event`  

The event that triggered the calling of the action method. You may specify nil for this parameter if you are calling this method directly, instead of in response to an event. For example, you might specify `nil` when changing the value of a control programmatically.

## Discussion

This method takes the provided information and forwards it to the singleton UIApplication object for dispatching. If you supplied a valid target object, the app calls the action method on that target object. If the target object is `nil`, the app searches the responder chain for an object that defines the method.

Subclasses may override this method and use it to observe or modify the action-dispatching behavior. Implementations need to call `super` when they want to continue with the execution of the action method.

## See Also

### Related Documentation

func addTarget(Any?, action: Selector, for: UIControl.Event)

Associates a target object and action method with the control.

### Triggering actions

func performPrimaryAction()

Calls the method associated with the control’s primary action.

func sendAction(UIAction)

func sendActions(for: UIControl.Event)

Calls the action methods associated with the specified events.

