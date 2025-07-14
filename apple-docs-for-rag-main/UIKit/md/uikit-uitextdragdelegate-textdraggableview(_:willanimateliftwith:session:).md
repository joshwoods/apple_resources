

- UIKit
- UITextDragDelegate
-  textDraggableView(\_:willAnimateLiftWith:session:) 

Instance Method

# textDraggableView(\_:willAnimateLiftWith:session:)

Tells the delegate when the lift animation is about to begin, and gives you a chance to animate additional changes alongside the system animation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textDraggableView(
    _ textDraggableView: any UIView & UITextDraggable,
    willAnimateLiftWith animator: any UIDragAnimating,
    session: any UIDragSession
)
```

## Parameters 

`textDraggableView`  

The text view where the drag activity was started.

`animator`  

The animator that you use when adding animations.

`session`  

The drag session of the current drag activity.

## Discussion

You implement this delegate method when you want to add animations that happen alongside the system animation during the lift activity. To add such an animation, use the animator’s addAnimations(_:) method. To add an animation that happens after the system animation has ended, use the animator’s addCompletion(_:) method.

