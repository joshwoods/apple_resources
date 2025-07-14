

- AppKit
- NSSegmentedCell
-  selectSegment(withTag:) 

Instance Method

# selectSegment(withTag:)

Selects the segment with the specified tag.

macOS

``` source
@MainActor
func selectSegment(withTag tag: Int) -> Bool
```

## Parameters 

`tag`  

The tag associated with the desired segment.

## Return Value

true if the segment was selected successfully; otherwise, false.

## Discussion

Typically, you use Interface Builder to specify the tag for each segment. You may also set this value programmatically using the setTag(_:forSegment:) method.

## See Also

### Related Documentation

func setTag(Int, forSegment: Int)

Sets the tag for the specified segment.

### Specifying the Selected Segment

func setSelected(Bool, forSegment: Int)

Sets the selection state of the specified segment.

func makeNextSegmentKey()

Selects the next segment.

func makePreviousSegmentKey()

Selects the previous segment.

var selectedSegment: Int

The index of the selected segment of the control, or `-1` if no segment is selected.

func isSelected(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is selected,

