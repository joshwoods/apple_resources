

- AppKit
- NSSegmentedControl
-  setImageScaling(\_:forSegment:) 

Instance Method

# setImageScaling(\_:forSegment:)

Sets the scaling mode used to display the specified segment’s image.

macOS 10.5+

``` source
@MainActor
func setImageScaling(
    _ scaling: NSImageScaling,
    forSegment segment: Int
)
```

## Parameters 

`scaling`  

One of the image scaling constants. For a list of possible values, see NSImageScaling.

`segment`  

The index of the segment whose enabled state you want to get. This method raises an exception (rangeException) if the index is out of bounds.

## See Also

### Configuring a Segment Image

func setImage(NSImage?, forSegment: Int)

Sets the image for the specified segment.

func image(forSegment: Int) -> NSImage?

Returns the image associated with the specified segment.

func imageScaling(forSegment: Int) -> NSImageScaling

Returns the scaling mode used to display the specified segment’s image.

