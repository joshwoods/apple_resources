

- UIKit
- UIDragInteractionDelegate
-  dragInteraction(\_:willAnimateLiftWith:session:) 

Instance Method

# dragInteraction(\_:willAnimateLiftWith:session:)

Tells the delegate the system’s lift animation is about to start.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dragInteraction(
    _ interaction: UIDragInteraction,
    willAnimateLiftWith animator: any UIDragAnimating,
    session: any UIDragSession
)
```

## Parameters 

`interaction`  

The interaction that called this method.

`animator`  

The animator that provides custom animations to run alongside the system’s lift animation. You can also use it to add a completion block that runs after the animations have finished.

`session`  

The current drag session.

## Discussion

To add a custom animation block that runs during the lift animation, pass the block to the animator’s addAnimations(_:) method.

To add a completion block that runs after the lift animation has finished, pass the block to the animator’s addCompletion(_:) method.

## See Also

### Animating the drag behaviors

func dragInteraction(UIDragInteraction, item: UIDragItem, willAnimateCancelWith: any UIDragAnimating)

Tells the delegate the system’s cancellation animation is about to start.

