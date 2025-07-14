

- AppKit
- NSSegmentedControl
-  doubleValueForSelectedSegment 

Instance Property

# doubleValueForSelectedSegment

When the tracking mode for the control is set to use a momentary accelerator, returns a value for the selected segment.

macOS 10.10.3+

``` source
@MainActor
var doubleValueForSelectedSegment: Double { get }
```

## Return Value

The value of the selected segment interpreted as a double-precision floating-point number.

## Discussion

This method is intended for use with controls whose tracking mode is set to NSSegmentedControl.SwitchTracking.momentaryAccelerator. An assertion will occur if this method is called for other types of segmented controls.

## See Also

### Related Documentation

case momentaryAccelerator

On pressure-sensitive systems, when the user force clicks a segment, a momentary accelerator segmented control sends repeating actions as pressure changes occur. The control stops sending actions when the user releases pressure. A document-based app, for example, might implement a momentary accelerator segmented control in order to allow a user to adjust the speed of paging by using variable pressure. In this example, actions are sent to the app to indicate when pressure on the control has changed. The app then determines the amount of pressure currently applied, and adjusts navigation speed accordingly.

var trackingMode: NSSegmentedControl.SwitchTracking

The type of tracking behavior the control exhibits.

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

var selectedSegmentBezelColor: NSColor?

The color of the selected segment’s bezel, in appearances that support it.

