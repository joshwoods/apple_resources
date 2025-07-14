

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:failedToStartPictureInPictureWithError:) 

Instance Method

# playerViewController(\_:failedToStartPictureInPictureWithError:)

Tells the delegate when Picture in Picture fails to start.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    failedToStartPictureInPictureWithError error: any Error
)
```

## Parameters 

`playerViewController`  

The player view controller.

`error`  

An error object that describes the failure.

## See Also

### Responding to Picture in Picture Life Cycle Events

func playerViewControllerShouldAutomaticallyDismissAtPictureInPictureStart(AVPlayerViewController) -> Bool

Asks the delegate whether the player view controller automatically dismisses itself when Picture in Picture starts.

func playerViewControllerWillStartPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture is about to start.

func playerViewControllerDidStartPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture starts.

func playerViewControllerWillStopPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture is about to stop.

func playerViewControllerDidStopPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture stops.

func playerViewController(AVPlayerViewController, restoreUserInterfaceForPictureInPictureStopWithCompletionHandler: (Bool) -> Void)

Tells the delegate when Picture in Picture is about to stop so you can restore your app’s user interface.

