

- AppKit
- NSSegmentedControl
-  setImage(\_:forSegment:) 

Instance Method

# setImage(\_:forSegment:)

Sets the image for the specified segment.

macOS

``` source
@MainActor
func setImage(
    _ image: NSImage?,
    forSegment segment: Int
)
```

## Parameters 

`image`  

The image to apply to the segment or `nil` if you want to clear the existing image. Images are not scaled to fit inside a segment. If the image is larger than the available space, it is clipped.

`segment`  

The index of the segment whose image you want to set. This method raises an exception (rangeException) if the index is out of bounds.

## See Also

### Configuring a Segment Image

func image(forSegment: Int) -> NSImage?

Returns the image associated with the specified segment.

func setImageScaling(NSImageScaling, forSegment: Int)

Sets the scaling mode used to display the specified segment’s image.

func imageScaling(forSegment: Int) -> NSImageScaling

Returns the scaling mode used to display the specified segment’s image.

