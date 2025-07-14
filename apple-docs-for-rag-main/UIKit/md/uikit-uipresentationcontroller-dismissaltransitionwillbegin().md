

- UIKit
- UIPresentationController
-  dismissalTransitionWillBegin() 

Instance Method

# dismissalTransitionWillBegin()

Notifies the presentation controller that the dismissal animations are about to start.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func dismissalTransitionWillBegin()
```

## Discussion

The default implementation of this method does nothing. Subclasses can override this method and use it to configure any animations associated with your presentation’s custom views. To perform your animations, get the transition coordinator of the presented view controller and call its animate(alongsideTransition:completion:) or animateAlongsideTransition(in:animation:completion:) method. Calling those methods ensures that your animations are executed at the same time as any other transition animations.

Do not use this method to remove your views from the view hierarchy. Remove your views in the dismissalTransitionDidEnd(_:) method instead.

## See Also

### Tracking the transition’s start and end

func presentationTransitionWillBegin()

Notifies the presentation controller that the presentation animations are about to start.

func presentationTransitionDidEnd(Bool)

Notifies the presentation controller that the presentation animations finished.

func dismissalTransitionDidEnd(Bool)

Notifies the presentation controller that the dismissal animations finished.

