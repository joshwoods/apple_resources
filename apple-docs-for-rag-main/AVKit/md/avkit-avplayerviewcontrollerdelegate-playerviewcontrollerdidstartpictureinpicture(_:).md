

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewControllerDidStartPictureInPicture(\_:) 

Instance Method

# playerViewControllerDidStartPictureInPicture(\_:)

Tells the delegate when Picture in Picture starts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
optional func playerViewControllerDidStartPictureInPicture(_ playerViewController: AVPlayerViewController)
```

## Parameters 

`playerViewController`  

The player view controller.

## Mentioned in 

Adopting Picture in Picture in a Standard Player

## See Also

### Responding to Picture in Picture Life Cycle Events

func playerViewControllerShouldAutomaticallyDismissAtPictureInPictureStart(AVPlayerViewController) -> Bool

Asks the delegate whether the player view controller automatically dismisses itself when Picture in Picture starts.

func playerViewControllerWillStartPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture is about to start.

func playerViewController(AVPlayerViewController, failedToStartPictureInPictureWithError: any Error)

Tells the delegate when Picture in Picture fails to start.

func playerViewControllerWillStopPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture is about to stop.

func playerViewControllerDidStopPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture stops.

func playerViewController(AVPlayerViewController, restoreUserInterfaceForPictureInPictureStopWithCompletionHandler: (Bool) -> Void)

Tells the delegate when Picture in Picture is about to stop so you can restore your app’s user interface.

