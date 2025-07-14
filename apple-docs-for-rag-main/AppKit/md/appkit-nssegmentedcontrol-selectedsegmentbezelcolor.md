

- AppKit
- NSSegmentedControl
-  selectedSegmentBezelColor 

Instance Property

# selectedSegmentBezelColor

The color of the selected segment’s bezel, in appearances that support it.

macOS 10.12.2+

``` source
@NSCopying @MainActor
var selectedSegmentBezelColor: NSColor? { get set }
```

## See Also

### Managing the Selected Segment

var selectedSegment: Int

The index of the selected segment of the control, or `-1` if no segment is selected.

var indexOfSelectedItem: Int

func selectSegment(withTag: Int) -> Bool

Selects the segment with the specified tag.

func setSelected(Bool, forSegment: Int)

Sets the selection state of the specified segment.

func isSelected(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is selected.

var doubleValueForSelectedSegment: Double

When the tracking mode for the control is set to use a momentary accelerator, returns a value for the selected segment.

