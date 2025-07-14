

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:timeToSeekAfterUserNavigatedFrom:to:) 

Instance Method

# playerViewController(\_:timeToSeekAfterUserNavigatedFrom:to:)

Tells the delegate when the user skips, scrubs, or otherwise navigates to a new time and wants to resume playback at the target time.

tvOS 10.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    timeToSeekAfterUserNavigatedFrom oldTime: CMTime,
    to targetTime: CMTime
) -> CMTime
```

## Parameters 

`playerViewController`  

The player view controller.

`oldTime`  

The current playback time before the user began navigating.

`targetTime`  

The time to which the user navigated.

## Return Value

The time at which to begin playback.

## Mentioned in 

Working with Interstitial Content

## Discussion

The framework calls this method prior to beginning playback after a user-initiated scrubbing request. You can return a time value other than the specified target time if needed to enforce certain business rules. For instance, you may want to return a different time to prevent users from skipping past ad breaks in your program.

## See Also

### Responding to Navigation Events

func playerViewController(AVPlayerViewController, willResumePlaybackAfterUserNavigatedFrom: CMTime, to: CMTime)

Tells the delegate when the user navigates to a new time and playback is about to begin.

func skipToPreviousItem(for: AVPlayerViewController)

Tells the delegate when the user requests skipping to the previous item in the timeline.

func skipToNextItem(for: AVPlayerViewController)

Tells the delegate when the user requests skipping to the next item in the timeline.

