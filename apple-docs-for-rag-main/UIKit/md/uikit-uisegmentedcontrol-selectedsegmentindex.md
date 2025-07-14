

- UIKit
- UISegmentedControl
-  selectedSegmentIndex 

Instance Property

# selectedSegmentIndex

The index number that identifies the selected segment that the user last touched.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var selectedSegmentIndex: Int { get set }
```

## Discussion

The default value is noSegment (no segment selected) until the user touches a segment. Set this property to `-1` to turn off the current selection. UISegmentedControl ignores this property when isMomentary is true. When the user touches a segment to change the selection, the system generates the control event valueChanged. If you set up the segmented control to respond to this control event, it sends an action message to its target.

## See Also

### Managing segments

var numberOfSegments: Int

Returns the number of segments the segmented control has.

func segmentIndex(identifiedBy: UIAction.Identifier) -> Int

The index of a segment with an action that has an identifier matching the identifier you specify.

func insertSegment(action: UIAction, at: Int, animated: Bool)

Insert a segment with the action you specify at the given index.

func insertSegment(with: UIImage?, at: Int, animated: Bool)

Inserts a segment at the position you specify and gives it an image as content.

func insertSegment(withTitle: String?, at: Int, animated: Bool)

Inserts a segment at the position you specify and gives it a title as content.

func removeAllSegments()

Removes all segments of the segmented control.

func removeSegment(at: Int, animated: Bool)

Removes the segment you specify from the segmented control, optionally animating the transition.

class var noSegment: Int

A segment index value indicating that there’s no selected segment.

