

- UIKit
- UIPresentationController
-  dismissalTransitionDidEnd(\_:) 

Instance Method

# dismissalTransitionDidEnd(\_:)

Notifies the presentation controller that the dismissal animations finished.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func dismissalTransitionDidEnd(_ completed: Bool)
```

## Parameters 

`completed`  

true if the animations completed and the presented view controller was dismissed or false if the animations were canceled and the presented view controller is still visible.

## Discussion

The default implementation of this method does nothing. Subclasses can override this method and use it to remove any custom views that the presentation controller added to the view hierarchy. Remove your views only if the `completed` parameter is true.

## See Also

### Tracking the transition’s start and end

func presentationTransitionWillBegin()

Notifies the presentation controller that the presentation animations are about to start.

func presentationTransitionDidEnd(Bool)

Notifies the presentation controller that the presentation animations finished.

func dismissalTransitionWillBegin()

Notifies the presentation controller that the dismissal animations are about to start.

