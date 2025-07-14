

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:didPresent:) 

Instance Method

# playerViewController(\_:didPresent:)

Tells the delegate when the player view controller finishes playing a range of interstitial content.

iOS 16.0+iPadOS 16.0+tvOS 9.0+visionOS 1.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    didPresent interstitial: AVInterstitialTimeRange
)
```

## Parameters 

`playerViewController`  

The player view controller.

`interstitial`  

The time range of interstitial content that’s finished playback.

## Discussion

Interstitial content is material that’s unrelated to the main content and may have special playback options or requirements. For example, implement this method to record when a user begins viewing an advertisement, or to enable the player view controller’s requiresLinearPlayback property to prevent skipping mandatory legal notices.

Use the interstitialTimeRanges property to identify the time ranges of interstitial content in the media timeline.

## See Also

### Responding to Interstitial Content Playback Events

func playerViewController(AVPlayerViewController, willPresent: AVInterstitialTimeRange)

Tells the delegate when the player view controller is about to start playing a range of interstitial content.

