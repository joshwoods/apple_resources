

- UIKit
- UIResponder
-  pressesCancelled(\_:with:) 

Instance Method

# pressesCancelled(\_:with:)

Tells this object when a system event (such as a low-memory warning) cancels a press event.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func pressesCancelled(
    _ presses: Set,
    with event: UIPressesEvent?
)
```

## Parameters 

`presses`  

A set of UIPress instances that represent the presses associated with the event. The phase of each press is set to UIPress.Phase.cancelled.

`event`  

The event to which the presses belong.

## Discussion

UIKit calls this method when it receives a system interruption requiring cancellation of the press sequence. An interruption is anything that causes the application to become inactive or causes the view handling the press events to be removed from its window. Your implementation of this method should clean up any state associated with handling the press sequence. Failure to handle cancellation is likely to lead to incorrect behavior or crashes.

The default implementation of this method forwards the message up the responder chain. When creating your own subclasses, call `super` to forward any events that you don’t handle yourself.

## See Also

### Responding to press events

func pressesBegan(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a physical button is first pressed.

func pressesChanged(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a value associated with a press has changed.

func pressesEnded(Set&lt;UIPress>, with: UIPressesEvent?)

Tells the object when a button is released.

