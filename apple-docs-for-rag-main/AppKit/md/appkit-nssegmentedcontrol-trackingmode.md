

- AppKit
- NSSegmentedControl
-  trackingMode 

Instance Property

# trackingMode

The type of tracking behavior the control exhibits.

macOS 10.10.3+

``` source
@MainActor
var trackingMode: NSSegmentedControl.SwitchTracking { get set }
```

## Discussion

An NSSegmentedControl.SwitchTracking value specifies how the control responds when the user presses a keyboard key or clicks, force clicks (applies pressure in a pressure-sensitive system), releases pressure, and so on. For possible values see NSSegmentedControl.SwitchTracking.

## See Also

### Related Documentation

Segmented Control Programming Guide

var isContinuous: Bool

A Boolean value indicating whether the receiver’s cell sends its action message continuously to its target during mouse tracking.

var doubleValueForSelectedSegment: Double

When the tracking mode for the control is set to use a momentary accelerator, returns a value for the selected segment.

### Specifying the Segment Behavior

enum SwitchTracking

The following constants specify the type of tracking behavior a segmented control exhibits. They are used by trackingMode.

var segmentStyle: NSSegmentedControl.Style

The visual style used to display the control.

enum Style

The following constants specify the visual style used to display the segmented control. They are used by segmentStyle.

