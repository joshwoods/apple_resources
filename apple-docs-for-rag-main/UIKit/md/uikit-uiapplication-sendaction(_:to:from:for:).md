

- UIKit
- UIApplication
-  sendAction(\_:to:from:for:) 

Instance Method

# sendAction(\_:to:from:for:)

Sends an action message identified by the selector to a specified target.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func sendAction(
    _ action: Selector,
    to target: Any?,
    from sender: Any?,
    for event: UIEvent?
) -> Bool
```

## Parameters 

`action`  

A selector identifying an action method. See the discussion for information on the permitted selector forms.

`target`  

The object to receive the action message. If `target` is `nil`, the app sends the message to the first responder, from whence it progresses up the responder chain until it is handled.

`sender`  

The object that is sending the action message. The default sender is the UIControl object that invokes this method.

`event`  

A UIEvent object that encapsulates information about the event originating the action message.

## Return Value

true if a responder object handled the action message, false if no object in the responder chain handled the message.

## Discussion

Normally, this method is invoked by a UIControl object that the user has touched. The default implementation dispatches the action method to the given target object or, if no target is specified, to the first responder. Subclasses may override this method to perform special dispatching of action messages.

By default, this method pushes two parameters when calling the target. These last two parameters are optional for the receiver because it is up to the caller (usually a UIControl object) to remove any parameters it added. This design enables the action selector to be one of the following:

- `- (void)action`

- `- (void)action:(id)sender`

- `- (void)action:(id)sender forEvent:(UIEvent *)event`

## See Also

### Controlling and handling events

func sendEvent(UIEvent)

Dispatches an event to the appropriate responder objects in the app.

var applicationSupportsShakeToEdit: Bool

A Boolean value that determines whether shaking the device displays the undo-redo user interface.

