

- Media Player
- MPMoviePlayerController
-  cancelAllThumbnailImageRequests() Deprecated

Instance Method

# cancelAllThumbnailImageRequests()

Cancels all pending asynchronous thumbnail image requests.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func cancelAllThumbnailImageRequests()
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

This method cancels only requests made using the requestThumbnailImages(atTimes:timeOption:) method. It does not cancel requests made synchronously using the thumbnailImage(atTime:timeOption:) method.

## See Also

### Generating thumbnail images

func thumbnailImage(atTime: TimeInterval, timeOption: MPMovieTimeOption) -> UIImage!

Captures and returns a thumbnail image from the current movie.

Deprecated

func requestThumbnailImages(atTimes: [Any]!, timeOption: MPMovieTimeOption)

Captures one or more thumbnail images asynchronously from the current movie.

Deprecated

