

- UIKit
- UIPresentationController
-  presentationTransitionDidEnd(\_:) 

Instance Method

# presentationTransitionDidEnd(\_:)

Notifies the presentation controller that the presentation animations finished.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func presentationTransitionDidEnd(_ completed: Bool)
```

## Parameters 

`completed`  

true if the animations completed and the presented view controller is now visible or false if the animations were canceled and the presenting view controller is still visible.

## Discussion

The default implementation of this method does nothing. Subclasses can override this method and use it to perform any required cleanup. For example, if the completed parameter is false, you would use this method to remove your presentation’s custom views from the view hierarchy.

For an example of how to implement this method, see Add custom views to a presentation.

## See Also

### Tracking the transition’s start and end

func presentationTransitionWillBegin()

Notifies the presentation controller that the presentation animations are about to start.

func dismissalTransitionWillBegin()

Notifies the presentation controller that the dismissal animations are about to start.

func dismissalTransitionDidEnd(Bool)

Notifies the presentation controller that the dismissal animations finished.

