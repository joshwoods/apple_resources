

- AppKit
- NSSegmentedControl
-  imageScaling(forSegment:) 

Instance Method

# imageScaling(forSegment:)

Returns the scaling mode used to display the specified segment’s image.

macOS 10.5+

``` source
@MainActor
func imageScaling(forSegment segment: Int) -> NSImageScaling
```

## Parameters 

`segment`  

The index of the segment whose enabled state you want to get. This method raises an exception (rangeException) if the index is out of bounds.

## Return Value

One of the image scaling constants. For a list of possible values, see NSImageScaling. The default value is NSImageScaling.scaleProportionallyDown.

## See Also

### Configuring a Segment Image

func setImage(NSImage?, forSegment: Int)

Sets the image for the specified segment.

func image(forSegment: Int) -> NSImage?

Returns the image associated with the specified segment.

func setImageScaling(NSImageScaling, forSegment: Int)

Sets the scaling mode used to display the specified segment’s image.

