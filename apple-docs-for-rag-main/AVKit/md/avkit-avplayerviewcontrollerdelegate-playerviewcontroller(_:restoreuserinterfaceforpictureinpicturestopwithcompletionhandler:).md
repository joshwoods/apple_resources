

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:restoreUserInterfaceForPictureInPictureStopWithCompletionHandler:) 

Instance Method

# playerViewController(\_:restoreUserInterfaceForPictureInPictureStopWithCompletionHandler:)

Tells the delegate when Picture in Picture is about to stop so you can restore your app’s user interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    restoreUserInterfaceForPictureInPictureStopWithCompletionHandler completionHandler: @escaping (Bool) -> Void
)
```

``` source
optional func playerViewControllerRestoreUserInterfaceForPictureInPictureStop(_ playerViewController: AVPlayerViewController) async -> Bool
```

## Parameters 

`playerViewController`  

The player view controller.

`completionHandler`  

You must call the completion handler with a value of true to allow the system to finish restoring your app’s user interface.

## Mentioned in 

Adopting Picture in Picture in a Standard Player

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func playerViewControllerRestoreUserInterfaceForPictureInPictureStop(_ playerViewController: AVPlayerViewController) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Implement this method to reestablish your playback user interface when PiP ends. The framework calls this method no matter how PiP ends, whether it’s because the user ended playback, the user tapped the button to return ongoing video playback to your app, or the video finished playing on its own.

## See Also

### Responding to Picture in Picture Life Cycle Events

func playerViewControllerShouldAutomaticallyDismissAtPictureInPictureStart(AVPlayerViewController) -> Bool

Asks the delegate whether the player view controller automatically dismisses itself when Picture in Picture starts.

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

