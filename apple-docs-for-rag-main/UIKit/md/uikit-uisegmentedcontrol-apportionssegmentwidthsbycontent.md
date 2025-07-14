

- UIKit
- UISegmentedControl
-  apportionsSegmentWidthsByContent 

Instance Property

# apportionsSegmentWidthsByContent

Indicates whether the control attempts to adjust segment widths based on their content widths.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var apportionsSegmentWidthsByContent: Bool { get set }
```

## Discussion

If the value of this property is true, for segments whose width value is `0`, the control attempts to adjust segment widths based on their content widths.

The default is false.

## See Also

### Managing segment behavior and appearance

var isMomentary: Bool

A Boolean value that determines whether segments in the segmented control show selected state.

func setEnabled(Bool, forSegmentAt: Int)

Enables the segment you specify.

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

