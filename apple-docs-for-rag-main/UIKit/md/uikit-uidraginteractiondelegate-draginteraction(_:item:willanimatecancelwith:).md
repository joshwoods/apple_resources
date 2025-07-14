

- UIKit
- UIDragInteractionDelegate
-  dragInteraction(\_:item:willAnimateCancelWith:) 

Instance Method

# dragInteraction(\_:item:willAnimateCancelWith:)

Tells the delegate the system’s cancellation animation is about to start.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dragInteraction(
    _ interaction: UIDragInteraction,
    item: UIDragItem,
    willAnimateCancelWith animator: any UIDragAnimating
)
```

## Parameters 

`interaction`  

The interaction that called this method.

`item`  

The current drag item.

`animator`  

The animator that provides custom animations to run alongside the system’s animation. You can also use it to add a completion block that runs after the animations have finished.

## Discussion

This method is called for each drag item, whether it is visible or not.

To add a custom animation block that runs during the cancellation animation, pass the block to the animator’s addAnimations(_:) method.

To add a completion block that runs after the cancellation animation has finished, pass the block to the animator’s addCompletion(_:) method.

## See Also

### Animating the drag behaviors

func dragInteraction(UIDragInteraction, willAnimateLiftWith: any UIDragAnimating, session: any UIDragSession)

Tells the delegate the system’s lift animation is about to start.

