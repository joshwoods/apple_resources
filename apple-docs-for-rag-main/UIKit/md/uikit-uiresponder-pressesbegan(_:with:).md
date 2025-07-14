

- UIKit
- UIResponder
-  pressesBegan(\_:with:) 

Instance Method

# pressesBegan(\_:with:)

Tells this object when a physical button is first pressed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func pressesBegan(
    _ presses: Set,
    with event: UIPressesEvent?
)
```

## Parameters 

`presses`  

A set of UIPress instances that represent the new presses that occurred. The phase of each press is set to UIPress.Phase.began.

`event`  

The event to which the presses belong.

## Mentioned in 

Handling key presses made on a physical keyboard

## Discussion

UIKit calls this method when a new button is pressed by the user. Use this method to determine which button was pressed and to take any needed actions.

The default implementation of this method forwards the message up the responder chain. When creating your own subclasses, call `super` to forward any events that you don’t handle yourself.

## See Also

### Responding to press events

func pressesChanged(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a value associated with a press has changed.

func pressesEnded(Set&lt;UIPress>, with: UIPressesEvent?)

Tells the object when a button is released.

func pressesCancelled(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a system event (such as a low-memory warning) cancels a press event.

