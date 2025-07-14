

- UIKit
- UISegmentedControl
-  setContentOffset(\_:forSegmentAt:) 

Instance Method

# setContentOffset(\_:forSegmentAt:)

Adjusts the offset for drawing the content (image or text) of the specified segment.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setContentOffset(
    _ offset: CGSize,
    forSegmentAt segment: Int
)
```

## Parameters 

`offset`  

The offset (as a CGSize type) from the origin of the segment at which to draw the segment’s content. The default offset is (0,0).

`segment`  

An index number identifying a segment in the control. It must be a number between 0 and the number of segments (numberOfSegments) minus 1; the segmented control pins values exceeding this upper range to the last segment.

## See Also

### Managing segment behavior and appearance

var isMomentary: Bool

A Boolean value that determines whether segments in the segmented control show selected state.

func setEnabled(Bool, forSegmentAt: Int)

Enables the segment you specify.

func isEnabledForSegment(at: Int) -> Bool

Returns whether the indicated segment is enabled.

func contentOffsetForSegment(at: Int) -> CGSize

Returns the offset for drawing the content (image or text) of the segment you specify.

func setWidth(CGFloat, forSegmentAt: Int)

Sets the width of the segment at the index you specify.

func widthForSegment(at: Int) -> CGFloat

Returns the width of the segment at the index you specify.

var apportionsSegmentWidthsByContent: Bool

Indicates whether the control attempts to adjust segment widths based on their content widths.

