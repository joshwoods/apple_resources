

- AppKit
- NSImageView
-  imageFrameStyle 

Instance Property

# imageFrameStyle

The style of frame that appears around the image.

macOS

``` source
@MainActor
var imageFrameStyle: NSImageView.FrameStyle { get set }
```

## Discussion

The default value of this property is NSImageView.FrameStyle.none.

## See Also

### Specifying the visual characteristics

var imageAlignment: NSImageAlignment

The alignment of the cell’s image inside the image view.

var imageScaling: NSImageScaling

The scaling mode applied to make the cell’s image fit the frame of the image view.

var animates: Bool

A Boolean value indicating whether the image view automatically plays animated images.

var contentTintColor: NSColor?

