

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewControllerShouldAutomaticallyDismissAtPictureInPictureStart(\_:) 

Instance Method

# playerViewControllerShouldAutomaticallyDismissAtPictureInPictureStart(\_:)

Asks the delegate whether the player view controller automatically dismisses itself when Picture in Picture starts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
optional func playerViewControllerShouldAutomaticallyDismissAtPictureInPictureStart(_ playerViewController: AVPlayerViewController) -> Bool
```

## Parameters 

`playerViewController`  

The player view controller.

## Return Value

true to indicate that the player view controller automatically dismisses itself; otherwise false.

## Discussion

Implement this method and return false to prevent the player view controller from automatically dismissing when Picture in Picture starts.

## See Also

### Responding to Picture in Picture Life Cycle Events

func playerViewControllerWillStartPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture is about to start.

func playerViewControllerDidStartPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture starts.

func playerViewController(AVPlayerViewController, failedToStartPictureInPictureWithError: any Error)

Tells the delegate when Picture in Picture fails to start.

func playerViewControllerWillStopPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture is about to stop.

func playerViewControllerDidStopPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture stops.

func playerViewController(AVPlayerViewController, restoreUserInterfaceForPictureInPictureStopWithCompletionHandler: (Bool) -> Void)

Tells the delegate when Picture in Picture is about to stop so you can restore your app’s user interface.

