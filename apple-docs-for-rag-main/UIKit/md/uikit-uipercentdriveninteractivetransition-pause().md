

- UIKit
- UIPercentDrivenInteractiveTransition
-  pause() 

Instance Method

# pause()

Pauses an interruptible transition animation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
func pause()
```

## Discussion

This is a convenience method that calls through to the pauseInteractiveTransition() method of the context object. You might call this method so that you can begin driving an animation interactively. For example, when the user’s finger touches the screen, your gesture handler would call this method to stop the animation and then use changes to the touch location to update the percentComplete property.

## See Also

### Managing a transition

func update(CGFloat)

Updates the completion percentage of the transition.

func cancel()

Notifies the system that user interactions canceled the transition.

func finish()

Notifies the system that user interactions signaled the completion of the transition.

