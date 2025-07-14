

- AppKit
- NSSegmentedCell
-  setSelected(\_:forSegment:) 

Instance Method

# setSelected(\_:forSegment:)

Sets the selection state of the specified segment.

macOS

``` source
@MainActor
func setSelected(
    _ selected: Bool,
    forSegment segment: Int
)
```

## Parameters 

`selected`  

true if you want to select the segment; otherwise, false.

`segment`  

The index of the segment whose selection state you want to set. This method raises an exception (rangeException) if the index is out of bounds.

## Discussion

If the control allows only a single selection, this method deselects any other selected segments.

If the trackingMode property of the segmented cell is set to NSSegmentedControl.SwitchTracking.momentary, then attempting to set the selected state of the segment will have no effect.

## See Also

### Specifying the Selected Segment

func selectSegment(withTag: Int) -> Bool

Selects the segment with the specified tag.

func makeNextSegmentKey()

Selects the next segment.

func makePreviousSegmentKey()

Selects the previous segment.

var selectedSegment: Int

The index of the selected segment of the control, or `-1` if no segment is selected.

func isSelected(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is selected,

