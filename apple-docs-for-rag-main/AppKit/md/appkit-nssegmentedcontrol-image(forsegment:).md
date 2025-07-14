

- AppKit
- NSSegmentedControl
-  image(forSegment:) 

Instance Method

# image(forSegment:)

Returns the image associated with the specified segment.

macOS

``` source
@MainActor
func image(forSegment segment: Int) -> NSImage?
```

## Parameters 

`segment`  

The index of the segment whose image you want to get. This method raises an exception (rangeException) if the index is out of bounds.

## Return Value

The image associated with the segment; otherwise, `nil`.

## See Also

### Configuring a Segment Image

func setImage(NSImage?, forSegment: Int)

Sets the image for the specified segment.

func setImageScaling(NSImageScaling, forSegment: Int)

Sets the scaling mode used to display the specified segment’s image.

func imageScaling(forSegment: Int) -> NSImageScaling

Returns the scaling mode used to display the specified segment’s image.

