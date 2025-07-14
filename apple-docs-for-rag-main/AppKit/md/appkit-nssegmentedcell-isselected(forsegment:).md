

- AppKit
- NSSegmentedCell
-  isSelected(forSegment:) 

Instance Method

# isSelected(forSegment:)

Returns a Boolean value indicating whether the specified segment is selected,

macOS

``` source
@MainActor
func isSelected(forSegment segment: Int) -> Bool
```

## Parameters 

`segment`  

The index of the segment whose selection state you want to get. This method raises an exception (rangeException) if the index is out of bounds.

## Return Value

true if the segment is selected; otherwise, false.

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

var selectedSegment: Int

The index of the selected segment of the control, or `-1` if no segment is selected.

