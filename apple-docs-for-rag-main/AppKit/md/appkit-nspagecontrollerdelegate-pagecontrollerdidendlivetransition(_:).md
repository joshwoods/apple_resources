

- AppKit
- NSPageControllerDelegate
-  pageControllerDidEndLiveTransition(\_:) 

Instance Method

# pageControllerDidEndLiveTransition(\_:)

This message is sent when a transition animation completes.

macOS 10.8+

``` source
@MainActor
optional func pageControllerDidEndLiveTransition(_ pageController: NSPageController)
```

## Parameters 

`pageController`  

The page controller.

## Discussion

This message is sent when a transition animation completes either via swipe gesture or one of the page controller’s target-action navigation methods.

Your content view is still hidden and you must call the completeTransition() method on `pageController` when your content is ready to show.

If completed successfully, a pageController(_:didTransitionTo:) will already have been sent.

## See Also

### Transition Notification

func pageControllerWillStartLiveTransition(NSPageController)

This message is sent when the user begins a transition.

func pageController(NSPageController, didTransitionTo: Any)

This message is sent when any page transition is completed.

