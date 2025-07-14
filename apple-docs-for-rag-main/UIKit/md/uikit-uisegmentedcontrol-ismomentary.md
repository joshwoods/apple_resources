

- UIKit
- UISegmentedControl
-  isMomentary 

Instance Property

# isMomentary

A Boolean value that determines whether segments in the segmented control show selected state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isMomentary: Bool { get set }
```

## Discussion

The default value of this property is false. If it’s set to true, segments in the control don’t show selected state and don’t update the value of selectedSegmentIndex after tracking ends.

## See Also

### Managing segment behavior and appearance

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

var apportionsSegmentWidthsByContent: Bool

Indicates whether the control attempts to adjust segment widths based on their content widths.

