

- AppKit
- NSImageView
-  imageScaling 

Instance Property

# imageScaling

The scaling mode applied to make the cell’s image fit the frame of the image view.

macOS

``` source
@MainActor
var imageScaling: NSImageScaling { get set }
```

## Discussion

The default value of this property is NSImageScaling.scaleProportionallyDown.

## See Also

### Specifying the visual characteristics

var imageFrameStyle: NSImageView.FrameStyle

The style of frame that appears around the image.

var imageAlignment: NSImageAlignment

The alignment of the cell’s image inside the image view.

var animates: Bool

A Boolean value indicating whether the image view automatically plays animated images.

var contentTintColor: NSColor?

