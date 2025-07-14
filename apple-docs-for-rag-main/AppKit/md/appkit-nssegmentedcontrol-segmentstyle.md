

- AppKit
- NSSegmentedControl
-  segmentStyle 

Instance Property

# segmentStyle

The visual style used to display the control.

macOS 10.5+

``` source
@MainActor
var segmentStyle: NSSegmentedControl.Style { get set }
```

## Discussion

An `NSSegmentStyle` value that specifies the visual display used by the control. For possible values, see NSSegmentedControl.Style.

## See Also

### Specifying the Segment Behavior

var trackingMode: NSSegmentedControl.SwitchTracking

The type of tracking behavior the control exhibits.

enum SwitchTracking

The following constants specify the type of tracking behavior a segmented control exhibits. They are used by trackingMode.

enum Style

The following constants specify the visual style used to display the segmented control. They are used by segmentStyle.

