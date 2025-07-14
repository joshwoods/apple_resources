

- UIKit
- UISegmentedControl
-  imageForSegment(at:) 

Instance Method

# imageForSegment(at:)

Returns the image for a specific segment.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func imageForSegment(at segment: Int) -> UIImage?
```

## Parameters 

`segment`  

An index number identifying a segment in the control. It must be a number between 0 and the number of segments (numberOfSegments) minus 1; the segmented control pins values exceeding this upper range to the last segment.

## Return Value

Returns the image assigned to the receiver as content. If there is no image, it returns `nil`.

## See Also

### Managing segment content

func setImage(UIImage?, forSegmentAt: Int)

Sets the content of a segment to a given image.

func setTitle(String?, forSegmentAt: Int)

Sets the title of a segment.

func titleForSegment(at: Int) -> String?

Returns the title of the specified segment.

