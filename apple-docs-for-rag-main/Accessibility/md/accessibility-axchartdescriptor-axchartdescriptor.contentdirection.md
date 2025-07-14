

- Accessibility
- AXChartDescriptor
-  AXChartDescriptor.ContentDirection 

Enumeration

# AXChartDescriptor.ContentDirection

A constant that describes the content direction of the chart.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum ContentDirection
```

## Overview

Use content direction to specify the direction of the x-axis, which the audio graph represents as time. For example, a bar chart might have a content direction of AXChartDescriptor.ContentDirection.leftToRight, and a pie chart might have a content direction of AXChartDescriptor.ContentDirection.radialClockwise.

## Topics

### Content directions

case leftToRight

A content direction with an x-axis that increases from left to right.

case rightToLeft

A content direction with an x-axis that increases from right to left.

case bottomToTop

A content direction with an x-axis that increases from bottom to top.

case topToBottom

A content direction with an x-axis that increases from top to bottom.

case radialClockwise

A content direction with a radial x-axis that increases clockwise.

case radialCounterClockwise

A content direction with a radial x-axis that increases counterclockwise.

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

### Specifying the content layout

var contentFrame: CGRect

The bounds of the view, in screen coordinates, for visually rendering data values.

var contentDirection: AXChartDescriptor.ContentDirection

The direction of the content in the chart.

