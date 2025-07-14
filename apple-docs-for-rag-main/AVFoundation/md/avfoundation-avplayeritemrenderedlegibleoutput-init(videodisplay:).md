

- AVFoundation
- AVPlayerItemRenderedLegibleOutput
-  init(videoDisplay:) 

Initializer

# init(videoDisplay:)

Creates a rendered legible output object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
init(videoDisplay videoDisplaySize: CGSize)
```

## Parameters 

`videoDisplaySize`  

The size of the video display.

## Discussion

You can also choose to reset the videoDisplaySize value after initialization or during playback.

Important

Attempting to set a video display size of zero results in the system throwing an exception.

