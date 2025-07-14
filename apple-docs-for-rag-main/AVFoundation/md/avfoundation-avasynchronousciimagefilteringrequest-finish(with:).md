

- AVFoundation
- AVAsynchronousCIImageFilteringRequest
-  finish(with:) 

Instance Method

# finish(with:)

Notifies AVFoundation that you cannot fulfill the image filtering request.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func finish(with error: any Error)
```

## Parameters 

`error`  

An error object describing the reason to

## Discussion

Call this method if you cannot process the input image and wish to abort playback as a result—for example, if the outputImage object from your filter chain is nil. (If instead you want to fall back to rendering an unfiltered image, call the finish(with:context:) and pass the sourceImage object to the `filteredImage` parameter.)

Calling this method causes AVFoundation to post a notification named failedToPlayToEndTimeNotification. Observers of this notification can use the AVPlayerItemFailedToPlayToEndTimeErrorKey key to examine the error you provide.

## See Also

### Returning the Filtered Image

func finish(with: CIImage, context: CIContext?)

Provides the filtered video frame image to AVFoundation for further processing or display.

