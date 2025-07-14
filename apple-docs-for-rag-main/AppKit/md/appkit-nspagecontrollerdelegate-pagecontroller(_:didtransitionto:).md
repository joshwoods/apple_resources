

- AppKit
- NSPageControllerDelegate
-  pageController(\_:didTransitionTo:) 

Instance Method

# pageController(\_:didTransitionTo:)

This message is sent when any page transition is completed.

macOS 10.8+

``` source
@MainActor
optional func pageController(
    _ pageController: NSPageController,
    didTransitionTo object: Any
)
```

## Parameters 

`pageController`  

The page controller.

`object`  

The object to display.

## See Also

### Transition Notification

func pageControllerWillStartLiveTransition(NSPageController)

This message is sent when the user begins a transition.

func pageControllerDidEndLiveTransition(NSPageController)

This message is sent when a transition animation completes.

