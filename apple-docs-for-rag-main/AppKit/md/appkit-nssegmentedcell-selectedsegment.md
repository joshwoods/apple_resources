

- AppKit
- NSSegmentedCell
-  selectedSegment 

Instance Property

# selectedSegment

The index of the selected segment of the control, or `-1` if no segment is selected.

macOS

``` source
@MainActor
var selectedSegment: Int { get set }
```

## Discussion

This property contains the zero-based index of the segment. If the control allows multiple selections, the value of this property is the index of the most recently selected segment.

If you specify an index that is out of bounds, an exception (rangeException) is raised.

## See Also

### Specifying the Selected Segment

func setSelected(Bool, forSegment: Int)

Sets the selection state of the specified segment.

func selectSegment(withTag: Int) -> Bool

Selects the segment with the specified tag.

func makeNextSegmentKey()

Selects the next segment.

func makePreviousSegmentKey()

Selects the previous segment.

func isSelected(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is selected,

