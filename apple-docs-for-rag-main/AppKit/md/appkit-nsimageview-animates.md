

- AppKit
- NSImageView
-  animates 

Instance Property

# animates

A Boolean value indicating whether the image view automatically plays animated images.

macOS

``` source
@MainActor
var animates: Bool { get set }
```

## Discussion

When the value of this property is true, the image view plays animated images automatically using the timing and looping characteristics stored in the image data. The default value of this property is true.

Decoding an animated GIF file is the only way to create an animated NSImage object. If the image view has been assigned an image that was created from animated GIF data, setting this property to true enables automatic playback of the animation. If this property is set to false, only the first frame of an animated image is displayed.

Loading an animated GIF file using an NSImage object produces an image that uses an NSBitmapImageRep object. The currentFrame, currentFrameDuration, and frameCount properties of the bitmap image representation determine the timing and looping characteristics of the animation. For more information, see NSBitmapImageRep.

## See Also

### Specifying the visual characteristics

var imageFrameStyle: NSImageView.FrameStyle

The style of frame that appears around the image.

var imageAlignment: NSImageAlignment

The alignment of the cell’s image inside the image view.

var imageScaling: NSImageScaling

The scaling mode applied to make the cell’s image fit the frame of the image view.

var contentTintColor: NSColor?

