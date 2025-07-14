

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:willBeginFullScreenPresentationWithAnimationCoordinator:) 

Instance Method

# playerViewController(\_:willBeginFullScreenPresentationWithAnimationCoordinator:)

Tells the delegate when the player view controller is about to start full-screen display.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    willBeginFullScreenPresentationWithAnimationCoordinator coordinator: any UIViewControllerTransitionCoordinator
)
```

## Parameters 

`playerViewController`  

The player view controller.

`coordinator`  

The transition coordinator to use when coordinating animations.

## Discussion

This method isn’t called if you embed the player view controller as a child of the presented view controller.

## See Also

### Responding to Full-Screen Presentations

func playerViewController(AVPlayerViewController, willEndFullScreenPresentationWithAnimationCoordinator: any UIViewControllerTransitionCoordinator)

Tells the delegate when the player view controller is about to end full-screen display.

func playerViewController(AVPlayerViewController, restoreUserInterfaceForFullScreenExitWithCompletionHandler: (Bool) -> Void)

Tells the delegate to restore the app’s user interface after returning from a full-screen presentation.

