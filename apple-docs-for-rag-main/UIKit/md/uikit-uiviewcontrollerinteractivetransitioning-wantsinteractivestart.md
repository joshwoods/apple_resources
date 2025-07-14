

- UIKit
- UIViewControllerInteractiveTransitioning
-  wantsInteractiveStart 

Instance Property

# wantsInteractiveStart

A Boolean value indicating whether the transition is interactive when it starts.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
optional var wantsInteractiveStart: Bool { get }
```

## Discussion

The value of this property is true when the transition is interactive from the moment it starts. The property is false when the transition starts off as noninteractive. However, even a transition that starts off as noninteractive may become interactive later if it implements the interruptibleAnimator(using:) method of the UIViewControllerAnimatedTransitioning protocol.

## See Also

### Starting an interactive transition

func startInteractiveTransition(any UIViewControllerContextTransitioning)

Called when the system needs to set up the interactive portions of a view controller transition and start the animations.

**Required**

