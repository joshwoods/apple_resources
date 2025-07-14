

- AppKit
- NSSegmentedControl
- NSSegmentedControl.SwitchTracking
-  NSSegmentedControl.SwitchTracking.momentaryAccelerator 

Case

# NSSegmentedControl.SwitchTracking.momentaryAccelerator

On pressure-sensitive systems, when the user force clicks a segment, a momentary accelerator segmented control sends repeating actions as pressure changes occur. The control stops sending actions when the user releases pressure. A document-based app, for example, might implement a momentary accelerator segmented control in order to allow a user to adjust the speed of paging by using variable pressure. In this example, actions are sent to the app to indicate when pressure on the control has changed. The app then determines the amount of pressure currently applied, and adjusts navigation speed accordingly.

macOS 10.10.3+

``` source
case momentaryAccelerator
```

## Discussion

When the control is configured as continuous (see isContinuous), the interval between repeating actions automatically adjusts to match the applied pressure. As the user presses harder, actions are sent more rapidly. As the user reduces pressure, actions slow down. As such, the user has direct control over how fast actions are sent. Continuous momentary accelerator segmented controls are intended for continuously advancing through a series of discrete objects, such as photos in an album or pages in a book.

When configured as noncontinuous, actions are sent whenever a change in pressure occurs. Noncontinuous momentary accelerator segmented controls are intended for adjusting the speed of navigation, such as playback speed in a media player, based on pressure. Once the control is released, a final action is sent.

When the user force clicks a segment in the control, selectedSegment value is the index of the active segment, and doubleValueForSelectedSegment is a measurement of pressure between `1.0` and approaching `2.0`. When the user releases pressure, the selectedSegment value is `-1` and doubleValueForSelectedSegment is `0.0`.

On a system that doesn’t support pressure sensitivity, a momentary accelerator segmented control behaves like a control of type NSSegmentedControl.SwitchTracking.momentary.

## See Also

### Constants

case selectOne

Only one segment in the control can be selected at a time.

case selectAny

One or more segment cells in the control can be selected at a time.

case momentary

A segment is selected only when the user is pressing the mouse down within the bounds of the segment. When the mouse is no longer down within the segment, the segment is automatically deselected. A momentary segmented control sends an action when the user clicks a segment, and another action when the user releases the segment. If configured as continuous (see isContinuous), the control also sends actions at repeating intervals until the user releases the segment, at which point the control sends its final action.

