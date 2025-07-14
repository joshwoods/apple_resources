

- AVKit
- AVPlayerViewControllerDelegate
-  skipToNextItem(for:) 

Instance Method

# skipToNextItem(for:)

Tells the delegate when the user requests skipping to the next item in the timeline.

tvOS 10.0+

``` source
optional func skipToNextItem(for playerViewController: AVPlayerViewController)
```

## Parameters 

`playerViewController`  

The player view controller.

## Discussion

The framework calls this method when you set the player view controller’s skipping behavior to AVPlayerViewControllerSkippingBehavior.skipItem and a user performs a forward skip gesture (by pressing the right side of the Siri Remote’s Touch surface). Implement this method to update the player view controller’s player to play the next player item.

## See Also

### Responding to Navigation Events

func playerViewController(AVPlayerViewController, timeToSeekAfterUserNavigatedFrom: CMTime, to: CMTime) -> CMTime

Tells the delegate when the user skips, scrubs, or otherwise navigates to a new time and wants to resume playback at the target time.

func playerViewController(AVPlayerViewController, willResumePlaybackAfterUserNavigatedFrom: CMTime, to: CMTime)

Tells the delegate when the user navigates to a new time and playback is about to begin.

func skipToPreviousItem(for: AVPlayerViewController)

Tells the delegate when the user requests skipping to the previous item in the timeline.

