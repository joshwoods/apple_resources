

- AppKit
- NSSplitView
-  NSSplitView.DividerStyle 

Enumeration

# NSSplitView.DividerStyle

Constants that specify the style of the split view’s dividers.

macOS 10.5+

``` source
enum DividerStyle
```

## Overview

These constants specify the possible divider styles that NSSplitView uses.

## Topics

### Constants

case thick

A thick style divider displays between subviews.

case thin

A thin style divider displays between subviews.

case paneSplitter

A thick style divider with a 3D appearance displays between subviews.

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

### Configuring and Drawing Dividers

var dividerStyle: NSSplitView.DividerStyle

The style of divider between views.

var dividerColor: NSColor

The color of the dividers that the split view draws between subviews.

var dividerThickness: CGFloat

The thickness of the dividers for the split view.

func drawDivider(in: NSRect)

Draws a divider between two of the split view’s subviews.

