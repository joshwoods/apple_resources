

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewControllerShouldDismiss(\_:) 

Instance Method

# playerViewControllerShouldDismiss(\_:)

Asks the delegate object whether the player view controller dismisses itself upon request.

tvOS 11.0+

``` source
optional func playerViewControllerShouldDismiss(_ playerViewController: AVPlayerViewController) -> Bool
```

## Parameters 

`playerViewController`  

The player view controller.

## Return Value

true if the player view controller should dismiss itself; otherwise false.

## Discussion

If allowed, the player view controller dismisses itself with animation. If you’ve embedded the player view controller in another view, the delegate may need to manually dismiss the view controller.

## See Also

### Dismissing the Player View Controller

func playerViewControllerWillBeginDismissalTransition(AVPlayerViewController)

Tells the delegate when the player view controller is about to start its dismissal transition.

func playerViewControllerDidEndDismissalTransition(AVPlayerViewController)

Tells the delegate when the player view controller ends its dismissal transition.

