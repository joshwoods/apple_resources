

- Metal Performance Shaders Graph
-  MPSGraphNonMaximumSuppressionCoordinateMode 

Enumeration

# MPSGraphNonMaximumSuppressionCoordinateMode

The non-maximum suppression coordinate mode.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MPSGraphNonMaximumSuppressionCoordinateMode
```

## Overview

The coordinate mode to use. At initialization defaults to MPSGraphNonMaximumSuppressionCoordinateModeCornersHeightFirst. This mode specifies the representation used for the 4 box coordinate values. Center coordinate modes define a centered box and the box dimensions.

```
CornersHeightFirst:
    [h_start, w_start, h_end, w_end]
CornersWidthFirst:
    [w_start, h_start, w_end, h_end]
CentersHeightFirst:
    [h_center, w_center, box_height, box_width]
CentersWidthFirst:
    [w_center, w_center, box_height, box_width]
```

## Topics

### Enumeration Cases

case centersHeightFirst

case centersWidthFirst

case cornersWidthFirst

case explicit

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

