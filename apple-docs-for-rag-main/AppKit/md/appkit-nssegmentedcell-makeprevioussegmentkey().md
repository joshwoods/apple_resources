

- AppKit
- NSSegmentedCell
-  makePreviousSegmentKey() 

Instance Method

# makePreviousSegmentKey()

Selects the previous segment.

macOS

``` source
@MainActor
func makePreviousSegmentKey()
```

## Discussion

The previous segment is the one to the left of the currently selected segment. For the first segment, the selection wraps around to the last segment of the control.

## See Also

### Specifying the Selected Segment

func setSelected(Bool, forSegment: Int)

Sets the selection state of the specified segment.

func selectSegment(withTag: Int) -> Bool

Selects the segment with the specified tag.

func makeNextSegmentKey()

Selects the next segment.

var selectedSegment: Int

The index of the selected segment of the control, or `-1` if no segment is selected.

func isSelected(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is selected,

