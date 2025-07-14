

- UIKit
- UISegmentedControl
-  insertSegment(with:at:animated:) 

Instance Method

# insertSegment(with:at:animated:)

Inserts a segment at the position you specify and gives it an image as content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func insertSegment(
    with image: UIImage?,
    at segment: Int,
    animated: Bool
)
```

## Parameters 

`image`  

An image object to use as the content of the segment.

`segment`  

An index number identifying a segment in the control.

`segment` must be a number in the range 0 to the number of segments (numberOfSegments) inclusive; the segmented control pins values exceeding this upper range to the last segment.

The segmented control inserts the new segment immediately before the designated one.

`animated`  

true if the insertion of the new segment must animate; otherwise, false.

## See Also

### Managing segments

var numberOfSegments: Int

Returns the number of segments the segmented control has.

func segmentIndex(identifiedBy: UIAction.Identifier) -> Int

The index of a segment with an action that has an identifier matching the identifier you specify.

func insertSegment(action: UIAction, at: Int, animated: Bool)

Insert a segment with the action you specify at the given index.

func insertSegment(withTitle: String?, at: Int, animated: Bool)

Inserts a segment at the position you specify and gives it a title as content.

func removeAllSegments()

Removes all segments of the segmented control.

func removeSegment(at: Int, animated: Bool)

Removes the segment you specify from the segmented control, optionally animating the transition.

var selectedSegmentIndex: Int

The index number that identifies the selected segment that the user last touched.

class var noSegment: Int

A segment index value indicating that there’s no selected segment.

