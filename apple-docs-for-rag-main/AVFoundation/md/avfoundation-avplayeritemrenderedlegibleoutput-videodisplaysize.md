

- AVFoundation
- AVPlayerItemRenderedLegibleOutput
-  videoDisplaySize 

Instance Property

# videoDisplaySize

Set the video display size to use for rendering of pixel buffers.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var videoDisplaySize: CGSize { get set }
```

## Discussion

The output renders the pixel buffers according to the width and height of display area. If you set this property during the presentation time of a vended caption image, the output vends a new image rendered at the new size.

Important

Attempting to set a video display size of zero results in the system throwing an exception.

## See Also

### Configuring an output

var advanceIntervalForDelegateInvocation: TimeInterval

Permits advance invocation of the associated delegate, if any.

