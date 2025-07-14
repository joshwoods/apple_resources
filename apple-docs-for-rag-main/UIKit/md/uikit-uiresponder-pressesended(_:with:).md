

- UIKit
- UIResponder
-  pressesEnded(\_:with:) 

Instance Method

# pressesEnded(\_:with:)

Tells the object when a button is released.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func pressesEnded(
    _ presses: Set,
    with event: UIPressesEvent?
)
```

## Parameters 

`presses`  

A set of UIPress instances that represent the buttons that the user is no longer pressing. The phase of each press is set to UIPress.Phase.ended.

`event`  

The event to which the presses belong.

## Mentioned in 

Handling key presses made on a physical keyboard

## Discussion

UIKit calls this method when the user stops pressing one or more buttons. Use this method to take any needed actions in response to the end of the press.The default implementation of this method forwards the message up the responder chain. When creating your own subclasses, call `super` to forward any events that you don’t handle yourself.

## See Also

### Responding to press events

func pressesBegan(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a physical button is first pressed.

func pressesChanged(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a value associated with a press has changed.

func pressesCancelled(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a system event (such as a low-memory warning) cancels a press event.

