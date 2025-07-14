

- UIKit
- UIViewControllerAnimatedTransitioning
-  animationEnded(\_:) 

Instance Method

# animationEnded(\_:)

Tells your animator object that the transition animations have finished.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional func animationEnded(_ transitionCompleted: Bool)
```

## Parameters 

`transitionCompleted`  

Contains the value true if the transition completed successfully and the new view controller is now displayed or false if the transition was canceled and the original view controller is still visible.

## Discussion

UIKit calls this method at the end of a transition to let you know the results. Use this method to perform any final cleanup operations required by your transition animator when the transition finishes.

## See Also

### Performing a transition

func animateTransition(using: any UIViewControllerContextTransitioning)

Tells your animator object to perform the transition animations.

**Required**

