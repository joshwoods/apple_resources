

- AppKit
-  NSSegmentedCell 

Class

# NSSegmentedCell

An `NSSegmentedCell` object implements the appearance and behavior of a horizontal button divided into multiple segments. This class is used in conjunction with the NSSegmentedControl class to implement a segmented control.

macOS

``` source
@MainActor
class NSSegmentedCell
```

## Overview

Use the methods of `NSSegmentedCell` to customize the attributes of a segmented control. To customize the appearance of individual segments, you can also subclass and override the drawSegment(_:inFrame:with:) method.

## Topics

### Specifying the Number of Segments

var segmentCount: Int

The number of segments in the segmented control.

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

func isSelected(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is selected,

### Specifying the Tracking Mode

var trackingMode: NSSegmentedControl.SwitchTracking

The tracking mode used for the segments of the control.

### Configuring Individual Segments

func setLabel(String, forSegment: Int)

Sets the label for the specified segment.

func label(forSegment: Int) -> String?

Returns the label of the specified segment.

func setImage(NSImage?, forSegment: Int)

Sets the image for the specified segment.

func image(forSegment: Int) -> NSImage?

Returns the image associated with the specified segment.

func setImageScaling(NSImageScaling, forSegment: Int)

Sets the image scaling mode for the specified segment.

func imageScaling(forSegment: Int) -> NSImageScaling

Returns the image scaling mode associated with the specified segment.

func setWidth(CGFloat, forSegment: Int)

Sets the width of the specified segment.

func width(forSegment: Int) -> CGFloat

Returns the width of the specified segment.

func setEnabled(Bool, forSegment: Int)

Sets the enabled state of the specified segment

func isEnabled(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is enabled.

func setMenu(NSMenu?, forSegment: Int)

Sets the menu for the specified segment.

func menu(forSegment: Int) -> NSMenu?

Returns the menu for the specified segment.

func setToolTip(String?, forSegment: Int)

Sets the tooltip for the specified segment.

func toolTip(forSegment: Int) -> String?

Returns the tooltip of the specified segment.

func setTag(Int, forSegment: Int)

Sets the tag for the specified segment.

func tag(forSegment: Int) -> Int

Returns the tag of the specified segment.

### Drawing Custom Content

func drawSegment(Int, inFrame: NSRect, with: NSView)

Draws the image and label of the segment in the specified view.

### Specifying Segment Visual Styles

func interiorBackgroundStyle(forSegment: Int) -> NSView.BackgroundStyle

Returns the interior background style for the specified segment.

var segmentStyle: NSSegmentedControl.Style

The visual style used to display the segmented control.

## Relationships

### Inherits From

- NSActionCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- Sendable

