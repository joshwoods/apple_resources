

- AppKit
- NSPageControllerDelegate
-  pageControllerWillStartLiveTransition(\_:) 

Instance Method

# pageControllerWillStartLiveTransition(\_:)

This message is sent when the user begins a transition.

macOS 10.8+

``` source
@MainActor
optional func pageControllerWillStartLiveTransition(_ pageController: NSPageController)
```

## Parameters 

`pageController`  

The page controller.

## Discussion

This message is sent when the user begins a transition whether via a swipe gesture of one of the page controller’s target-action navigation methods.

## See Also

### Transition Notification

func pageControllerDidEndLiveTransition(NSPageController)

This message is sent when a transition animation completes.

func pageController(NSPageController, didTransitionTo: Any)

This message is sent when any page transition is completed.

