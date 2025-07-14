

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewControllerWillBeginDismissalTransition(\_:) 

Instance Method

# playerViewControllerWillBeginDismissalTransition(\_:)

Tells the delegate when the player view controller is about to start its dismissal transition.

tvOS 11.0+

``` source
optional func playerViewControllerWillBeginDismissalTransition(_ playerViewController: AVPlayerViewController)
```

## Parameters 

`playerViewController`  

The player view controller.

## See Also

### Dismissing the Player View Controller

func playerViewControllerShouldDismiss(AVPlayerViewController) -> Bool

Asks the delegate object whether the player view controller dismisses itself upon request.

func playerViewControllerDidEndDismissalTransition(AVPlayerViewController)

Tells the delegate when the player view controller ends its dismissal transition.

