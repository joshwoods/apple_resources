

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:restoreUserInterfaceForFullScreenExitWithCompletionHandler:) 

Instance Method

# playerViewController(\_:restoreUserInterfaceForFullScreenExitWithCompletionHandler:)

Tells the delegate to restore the app’s user interface after returning from a full-screen presentation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    restoreUserInterfaceForFullScreenExitWithCompletionHandler completionHandler: @escaping (Bool) -> Void
)
```

``` source
optional func playerViewControllerRestoreUserInterfaceForFullScreenExit(_ playerViewController: AVPlayerViewController) async -> Bool
```

## Parameters 

`playerViewController`  

The player view controller.

`completionHandler`  

The completion handler to call for the system to finish restoring your user interface. You must invoke this callback with a value of true.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func playerViewControllerRestoreUserInterfaceForFullScreenExit(_ playerViewController: AVPlayerViewController) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Responding to Full-Screen Presentations

func playerViewController(AVPlayerViewController, willBeginFullScreenPresentationWithAnimationCoordinator: any UIViewControllerTransitionCoordinator)

Tells the delegate when the player view controller is about to start full-screen display.

func playerViewController(AVPlayerViewController, willEndFullScreenPresentationWithAnimationCoordinator: any UIViewControllerTransitionCoordinator)

Tells the delegate when the player view controller is about to end full-screen display.

