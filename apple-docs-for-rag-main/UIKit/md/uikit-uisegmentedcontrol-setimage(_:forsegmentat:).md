

- UIKit
- UISegmentedControl
-  setImage(\_:forSegmentAt:) 

Instance Method

# setImage(\_:forSegmentAt:)

Sets the content of a segment to a given image.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setImage(
    _ image: UIImage?,
    forSegmentAt segment: Int
)
```

## Parameters 

`image`  

An image object to display in the segment. .

`segment`  

An index number identifying a segment in the control. It must be a number between 0 and the number of segments (numberOfSegments) minus 1; the segmented control pins values exceeding this upper range to the last segment.

## Discussion

A segment can have only an image or a title; it can’t have both. There’s no default image.

## See Also

### Managing segment content

func imageForSegment(at: Int) -> UIImage?

Returns the image for a specific segment.

func setTitle(String?, forSegmentAt: Int)

Sets the title of a segment.

func titleForSegment(at: Int) -> String?

Returns the title of the specified segment.

