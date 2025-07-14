

- UIKit
- UIResponder
-  pressesChanged(\_:with:) 

Instance Method

# pressesChanged(\_:with:)

Tells this object when a value associated with a press has changed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func pressesChanged(
    _ presses: Set,
    with event: UIPressesEvent?
)
```

## Parameters 

`presses`  

A set of UIPress instances containing changed values.

`event`  

The event to which the presses belong.

## Discussion

UIKit calls this method when an analog value associated with a button or thumbstick changes. For example, it calls this method when the analog force value of a push button changes. Use this method to take any needed actions in response to the change.

The default implementation of this method forwards the message up the responder chain. When creating your own subclasses, call `super` to forward any events that you don’t handle yourself.

## See Also

### Responding to press events

func pressesBegan(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a physical button is first pressed.

func pressesEnded(Set&lt;UIPress>, with: UIPressesEvent?)

Tells the object when a button is released.

func pressesCancelled(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a system event (such as a low-memory warning) cancels a press event.

