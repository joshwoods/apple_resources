

- UIKit
- UIPresentationController
-  presentationTransitionWillBegin() 

Instance Method

# presentationTransitionWillBegin()

Notifies the presentation controller that the presentation animations are about to start.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func presentationTransitionWillBegin()
```

## Discussion

The default implementation of this method does nothing. Subclasses can override it and use it to add custom views to the view hierarchy and to create any animations associated with those views. To perform your animations, get the transition coordinator of the presented view controller and call its animate(alongsideTransition:completion:) or animateAlongsideTransition(in:animation:completion:) method. Calling those methods ensures that your animations are executed at the same time as any other transition animations.

For an example of how to implement this method, see Add custom views to a presentation.

## See Also

### Tracking the transition’s start and end

func presentationTransitionDidEnd(Bool)

Notifies the presentation controller that the presentation animations finished.

func dismissalTransitionWillBegin()

Notifies the presentation controller that the dismissal animations are about to start.

func dismissalTransitionDidEnd(Bool)

Notifies the presentation controller that the dismissal animations finished.

