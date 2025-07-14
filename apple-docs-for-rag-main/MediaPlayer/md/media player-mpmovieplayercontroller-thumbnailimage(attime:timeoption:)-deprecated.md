

- Media Player
- MPMoviePlayerController
-  thumbnailImage(atTime:timeOption:) Deprecated

Instance Method

# thumbnailImage(atTime:timeOption:)

Captures and returns a thumbnail image from the current movie.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func thumbnailImage(
    atTime playbackTime: TimeInterval,
    timeOption option: MPMovieTimeOption
) -> UIImage!
```

Deprecated

Use AVPlayerViewController in AVKit

## Parameters 

`playbackTime`  

The time at which to capture the thumbnail image. The time value represents the number of seconds from the beginning of the current movie.

`option`  

The option to use when determining which specific frame to use for the thumbnail image. For a list of possible values, see MPMovieTimeOption.

## Return Value

An image object containing the image from the movie or `nil` if the thumbnail could not be captured.

## Discussion

This method captures the thumbnail image synchronously from the current movie (which is accessible from the MPMovieSourceType.unknown property).

Note

This method is not successful when the source URL is an HTTP Live Streaming (HLS) content source. The returned value for an HLS source is an empty `UIImage` object. See HTTP Live Streaming Overview.

## See Also

### Generating thumbnail images

func requestThumbnailImages(atTimes: [Any]!, timeOption: MPMovieTimeOption)

Captures one or more thumbnail images asynchronously from the current movie.

Deprecated

func cancelAllThumbnailImageRequests()

Cancels all pending asynchronous thumbnail image requests.

Deprecated

