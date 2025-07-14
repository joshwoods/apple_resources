

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:skipToNextChannel:) 

Instance Method

# playerViewController(\_:skipToNextChannel:)

Tells the delegate when the user wants to skip to the next channel.

tvOS 13.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    skipToNextChannel completion: @escaping (Bool) -> Void
)
```

``` source
optional func playerViewControllerSkipToNextChannel(_ playerViewController: AVPlayerViewController) async -> Bool
```

## Parameters 

`playerViewController`  

The player view controller.

`completion`  

A completion callback to invoke to dismiss the channel’s interstitial view.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func playerViewControllerSkipToNextChannel(_ playerViewController: AVPlayerViewController) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

To enable channel skipping, adopt this method and replace the current player item with one that reflects the next channel’s content, and call the completion handler to dismiss the channel’s interstitial view. Each call to this method should advance one channel, relative to the previous request, even if the prior request hasn’t yet completed.

Important

Only live video streams support channel skipping. This feature isn’t supported for VOD streams or local media.

## See Also

### Responding to Channel Changes

func playerViewController(AVPlayerViewController, skipToPreviousChannel: (Bool) -> Void)

Tells the delegate when the user wants to skip to the previous channel.

func nextChannelInterstitialViewController(for: AVPlayerViewController) -> UIViewController

Asks the delegate for a view controller that describes the layout of the next channel’s interstitial view.

func previousChannelInterstitialViewController(for: AVPlayerViewController) -> UIViewController

Asks the delegate for a view controller that describes the layout of the previous channel’s interstitial view.

