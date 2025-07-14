

- UIKit
- UISegmentedControl
-  setEnabled(\_:forSegmentAt:) 

Instance Method

# setEnabled(\_:forSegmentAt:)

Enables the segment you specify.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setEnabled(
    _ enabled: Bool,
    forSegmentAt segment: Int
)
```

## Parameters 

`enabled`  

true to enable the segment you specify or false to disable the segment. true by default.

`segment`  

An index number identifying a segment in the control. It must be a number between 0 and the number of segments (numberOfSegments) minus 1; the segmented control pins values exceeding this upper range to the last segment.

## See Also

### Managing segment behavior and appearance

var isMomentary: Bool

A Boolean value that determines whether segments in the segmented control show selected state.

func isEnabledForSegment(at: Int) -> Bool

Returns whether the indicated segment is enabled.

func setContentOffset(CGSize, forSegmentAt: Int)

Adjusts the offset for drawing the content (image or text) of the specified segment.

func contentOffsetForSegment(at: Int) -> CGSize

Returns the offset for drawing the content (image or text) of the segment you specify.

func setWidth(CGFloat, forSegmentAt: Int)

Sets the width of the segment at the index you specify.

func widthForSegment(at: Int) -> CGFloat

Returns the width of the segment at the index you specify.

var apportionsSegmentWidthsByContent: Bool

Indicates whether the control attempts to adjust segment widths based on their content widths.

