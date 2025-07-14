

- AVKit
- AVPlayerViewControllerDelegate
-  previousChannelInterstitialViewController(for:) 

Instance Method

# previousChannelInterstitialViewController(for:)

Asks the delegate for a view controller that describes the layout of the previous channel’s interstitial view.

tvOS 13.0+

``` source
optional func previousChannelInterstitialViewController(for playerViewController: AVPlayerViewController) -> UIViewController
```

## Parameters 

`playerViewController`  

The player view controller.

## Discussion

The framework calls this method when the user initiates, but hasn’t yet committed, a change in channel. The framework may call this method while a previous channel’s interstitial view is visible (on screen, or transitioning).

Important

Only live video streams support channel skipping. This feature isn’t supported for VOD streams or local media.

## See Also

### Responding to Channel Changes

func playerViewController(AVPlayerViewController, skipToNextChannel: (Bool) -> Void)

Tells the delegate when the user wants to skip to the next channel.

func playerViewController(AVPlayerViewController, skipToPreviousChannel: (Bool) -> Void)

Tells the delegate when the user wants to skip to the previous channel.

func nextChannelInterstitialViewController(for: AVPlayerViewController) -> UIViewController

Asks the delegate for a view controller that describes the layout of the next channel’s interstitial view.

