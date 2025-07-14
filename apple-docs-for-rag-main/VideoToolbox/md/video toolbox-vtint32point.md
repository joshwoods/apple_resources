

- Video Toolbox
-  VTInt32Point 

Structure

# VTInt32Point

A structure that represents a 32-bit integer point value.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
struct VTInt32Point
```

## Overview

Use this structure to represent a point at an (x, y) location.

## Topics

### Creating a Point

init()

Creates a size with coordinates equal to zero.

init(x: Int32, y: Int32)

Creates a point with coordinates specified as integer values.

### Accessing the Coordinates

var x: Int32

The x-coordinate of the point.

var y: Int32

The y-coordinate of the point.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

VTSession

An abstract object that provides the common interface to configure VideoToolbox session objects.

struct VTInt32Size

A structure that represents a 32-bit integer size value.

var VT_SUPPORT_COLORSYNC_PIXEL_TRANSFER: Bool

