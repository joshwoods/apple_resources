

- AppKit
- NSSegmentedCell
-  segmentStyle 

Instance Property

# segmentStyle

The visual style used to display the segmented control.

macOS 10.5+

``` source
@MainActor
var segmentStyle: NSSegmentedControl.Style { get set }
```

## Discussion

This property contains an `NSSegmentStyle` value that specifies the visual display used by the control.

## See Also

### Related Documentation

enum Style

The following constants specify the visual style used to display the segmented control. They are used by segmentStyle.

### Specifying Segment Visual Styles

func interiorBackgroundStyle(forSegment: Int) -> NSView.BackgroundStyle

Returns the interior background style for the specified segment.

