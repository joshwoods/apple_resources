

- UIKit
- UIResponder
-  motionBegan(\_:with:) 

Instance Method

# motionBegan(\_:with:)

Tells the responder that a motion event has begun.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func motionBegan(
    _ motion: UIEvent.EventSubtype,
    with event: UIEvent?
)
```

## Parameters 

`motion`  

An event-subtype constant indicating the kind of motion. A common motion is shaking, which is indicated by UIEvent.EventSubtype.motionShake.

`event`  

An object representing the event associated with the motion.

## Discussion

UIKit informs the responder only when a motion event starts and ends. It doesn’t report intermediate shakes. Motion events are delivered initially to the first responder and are forwarded up the responder chain as appropriate.

The default implementation of this method forwards the message up the responder chain.

## See Also

### Responding to motion events

func motionEnded(UIEvent.EventSubtype, with: UIEvent?)

Tells the responder that a motion event has ended.

func motionCancelled(UIEvent.EventSubtype, with: UIEvent?)

Tells the responder that a motion event has been canceled.

