

- Media Player
- MPMoviePlayerController
-  requestThumbnailImages(atTimes:timeOption:) Deprecated

Instance Method

# requestThumbnailImages(atTimes:timeOption:)

Captures one or more thumbnail images asynchronously from the current movie.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func requestThumbnailImages(
    atTimes playbackTimes: [Any]!,
    timeOption option: MPMovieTimeOption
)
```

Deprecated

Use AVPlayerViewController in AVKit

## Parameters 

`playbackTimes`  

An array of NSNumber objects containing the times at which to capture the thumbnail images. Each time value represents the number of seconds from the beginning of the current movie.

`option`  

The option to use when determining which specific frame to use for each thumbnail image. For a list of possible values, see MPMovieTimeOption.

## Discussion

This method processes each thumbnail request separately and asynchronously. When the results for a single image arrive, the movie player posts a MPMoviePlayerThumbnailImageRequestDidFinishNotification notification with the results for that image. Notifications are posted regardless of whether the image capture was successful or failed. You should register for this notification prior to calling this method.

Note

This method is not not called when the source URL is an HTTP Live Streaming (HLS) content source. See HTTP Live Streaming Overview.

## See Also

### Generating thumbnail images

func thumbnailImage(atTime: TimeInterval, timeOption: MPMovieTimeOption) -> UIImage!

Captures and returns a thumbnail image from the current movie.

Deprecated

func cancelAllThumbnailImageRequests()

Cancels all pending asynchronous thumbnail image requests.

Deprecated

