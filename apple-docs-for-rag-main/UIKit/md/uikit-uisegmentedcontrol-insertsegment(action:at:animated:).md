

- UIKit
- UISegmentedControl
-  insertSegment(action:at:animated:) 

Instance Method

# insertSegment(action:at:animated:)

Insert a segment with the action you specify at the given index.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
func insertSegment(
    action: UIAction,
    at segment: Int,
    animated: Bool
)
```

## Parameters 

`action`  

A UIAction object to set on the segment at the index you specify.

`segment`  

An unsigned integer index of a segment.

`animated`  

true if the insertion of the new segment animates; otherwise, false.

## Discussion

Segments prefer images over titles when the action contains both. Selecting a segment invokes the action’s UIActionHandler, as well as handlers for the valueChanged and primaryActionTriggered control events.

If a segment exists with the action’s identifier, this method updates the existing segment is if the index is the same or removes the segment if the index is different.

## See Also

### Managing segments

var numberOfSegments: Int

Returns the number of segments the segmented control has.

func segmentIndex(identifiedBy: UIAction.Identifier) -> Int

The index of a segment with an action that has an identifier matching the identifier you specify.

func insertSegment(with: UIImage?, at: Int, animated: Bool)

Inserts a segment at the position you specify and gives it an image as content.

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

