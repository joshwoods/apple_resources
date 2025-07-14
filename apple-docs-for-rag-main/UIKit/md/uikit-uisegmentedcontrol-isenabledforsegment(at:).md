

- UIKit
- UISegmentedControl
-  isEnabledForSegment(at:) 

Instance Method

# isEnabledForSegment(at:)

Returns whether the indicated segment is enabled.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func isEnabledForSegment(at segment: Int) -> Bool
```

## Parameters 

`segment`  

An index number identifying a segment in the control. It must be a number between 0 and the number of segments (numberOfSegments) minus 1; the segmented control pins values exceeding this upper range to the last segment.

## Return Value

true if the given segment is enabled and false if the segment is disabled. By default, segments are enabled.

## See Also

### Managing segment behavior and appearance

var isMomentary: Bool

A Boolean value that determines whether segments in the segmented control show selected state.

func setEnabled(Bool, forSegmentAt: Int)

Enables the segment you specify.

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

