

- AppKit
- NSSegmentedCell
-  makeNextSegmentKey() 

Instance Method

# makeNextSegmentKey()

Selects the next segment.

macOS

``` source
@MainActor
func makeNextSegmentKey()
```

## Discussion

The next segment is the one to the right of the currently selected segment. For the last segment, the selection wraps back to the beginning of the control.

## See Also

### Specifying the Selected Segment

func setSelected(Bool, forSegment: Int)

Sets the selection state of the specified segment.

func selectSegment(withTag: Int) -> Bool

Selects the segment with the specified tag.

func makePreviousSegmentKey()

Selects the previous segment.

var selectedSegment: Int

The index of the selected segment of the control, or `-1` if no segment is selected.

func isSelected(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is selected,

