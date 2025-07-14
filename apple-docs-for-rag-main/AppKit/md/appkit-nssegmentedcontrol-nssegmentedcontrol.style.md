

- AppKit
- NSSegmentedControl
-  NSSegmentedControl.Style 

Enumeration

# NSSegmentedControl.Style

The following constants specify the visual style used to display the segmented control. They are used by segmentStyle.

macOS 10.5+

``` source
enum Style
```

## Topics

### Constants

case automatic

The appearance of the segmented control is automatically determined based on the type of window in which the control is displayed and the position within the window.

case rounded

The control is displayed using the rounded style.

case texturedRounded

The control is displayed using the textured rounded style. In macOS 10.7 and later, this style uses the artwork defined for NSSegmentedControl.Style.texturedSquare, so you should specify NSSegmentedControl.Style.texturedSquare instead.

case roundRect

The control is displayed using the round rect style.

case texturedSquare

The control is displayed using the textured square style.

case capsule

The control is displayed using the capsule style. In macOS 10.7 and later, this style uses the artwork defined for NSSegmentedControl.Style.texturedSquare, so you should specify NSSegmentedControl.Style.texturedSquare instead.

case smallSquare

The control is displayed using the small square style.

case separated

The segments in the control are displayed very close to each other but not touching. For example, Safari in macOS 10.10 and later uses this style for the previous and next page segmented control.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the Segment Behavior

var trackingMode: NSSegmentedControl.SwitchTracking

The type of tracking behavior the control exhibits.

enum SwitchTracking

The following constants specify the type of tracking behavior a segmented control exhibits. They are used by trackingMode.

var segmentStyle: NSSegmentedControl.Style

The visual style used to display the control.

