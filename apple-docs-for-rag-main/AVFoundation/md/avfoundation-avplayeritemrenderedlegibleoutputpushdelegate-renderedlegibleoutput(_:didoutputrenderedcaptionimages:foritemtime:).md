

- AVFoundation
- AVPlayerItemRenderedLegibleOutputPushDelegate
-  renderedLegibleOutput(\_:didOutputRenderedCaptionImages:forItemTime:) 

Instance Method

# renderedLegibleOutput(\_:didOutputRenderedCaptionImages:forItemTime:)

Tells the delegate that new rendered caption images are available.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
optional func renderedLegibleOutput(
    _ output: AVPlayerItemRenderedLegibleOutput,
    didOutputRenderedCaptionImages captionImages: [AVRenderedCaptionImage],
    forItemTime itemTime: CMTime
)
```

## Parameters 

`output`  

The rendered legible output object.

`captionImages`  

An array of AVRenderedCaptionImage objects. A caption object consists of a CVPixelBuffer and its associated position, in pixels, relative to the video frame.

`itemTime`  

The item time at which to present the caption images.

