

- UIKit
- UIApplication
-  sendEvent(\_:) 

Instance Method

# sendEvent(\_:)

Dispatches an event to the appropriate responder objects in the app.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func sendEvent(_ event: UIEvent)
```

## Parameters 

`event`  

A UIEvent object encapsulating the information about an event, including the touches involved.

## Discussion

If you require it, you can intercept incoming events by subclassing UIApplication and overriding this method. For every event you intercept, you must dispatch it by calling `[super sendEvent:event]` after handling the event in your implementation.

## See Also

### Controlling and handling events

func sendAction(Selector, to: Any?, from: Any?, for: UIEvent?) -> Bool

Sends an action message identified by the selector to a specified target.

var applicationSupportsShakeToEdit: Bool

A Boolean value that determines whether shaking the device displays the undo-redo user interface.

