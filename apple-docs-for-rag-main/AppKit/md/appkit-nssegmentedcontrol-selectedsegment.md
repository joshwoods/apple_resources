

- AppKit
- NSSegmentedControl
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

If the control allows multiple selections, this property contains the most recently selected segment. If the index is out of bounds, an exception (rangeException) is raised.

## See Also

### Managing the Selected Segment

var indexOfSelectedItem: Int

func selectSegment(withTag: Int) -> Bool

Selects the segment with the specified tag.

func setSelected(Bool, forSegment: Int)

Sets the selection state of the specified segment.

func isSelected(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is selected.

var selectedSegmentBezelColor: NSColor?

The color of the selected segment’s bezel, in appearances that support it.

var doubleValueForSelectedSegment: Double

When the tracking mode for the control is set to use a momentary accelerator, returns a value for the selected segment.

