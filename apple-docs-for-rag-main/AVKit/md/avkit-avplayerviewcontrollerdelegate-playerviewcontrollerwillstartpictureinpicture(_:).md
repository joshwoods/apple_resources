

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewControllerWillStartPictureInPicture(\_:) 

Instance Method

# playerViewControllerWillStartPictureInPicture(\_:)

Tells the delegate when Picture in Picture is about to start.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
optional func playerViewControllerWillStartPictureInPicture(_ playerViewController: AVPlayerViewController)
```

## Parameters 

`playerViewController`  

The player view controller.

## Mentioned in 

Adopting Picture in Picture in a Standard Player

## Discussion

Implement this method to update your player user interface, such as hiding or disabling playback controls, prior to PiP starting.

## See Also

### Responding to Picture in Picture Life Cycle Events

func playerViewControllerShouldAutomaticallyDismissAtPictureInPictureStart(AVPlayerViewController) -> Bool

Asks the delegate whether the player view controller automatically dismisses itself when Picture in Picture starts.

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

