

- Video Toolbox
-  VTInt32Size 

Structure

# VTInt32Size

A structure that represents a 32-bit integer size value.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
struct VTInt32Size
```

## Overview

Use this structure to represent a size with a particular width and height.

## Topics

### Creating a Size

init()

Creates a size with a width and height of zero.

init(width: Int32, height: Int32)

Creates a size with a width and height.

### Accessing the Dimensions

var width: Int32

The width of the size.

var height: Int32

The height of the size.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

VTSession

An abstract object that provides the common interface to configure VideoToolbox session objects.

struct VTInt32Point

A structure that represents a 32-bit integer point value.

var VT_SUPPORT_COLORSYNC_PIXEL_TRANSFER: Bool

