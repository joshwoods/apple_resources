

- AppKit
- NSBezierPath
-  NSBezierPath.ElementType 

Enumeration

# NSBezierPath.ElementType

Constants that specify basic path element commands.

macOS

``` source
enum ElementType
```

## Overview

These commands are enough to define all of the possible path shapes. Each command has one or more points that contain information needed to position the path element. Most path elements use the current drawing point as the starting point for drawing. For more details, see Paths.

## Topics

### Constants

case moveTo

Moves the path object’s current drawing point to the specified point.

case lineTo

Creates a straight line from the current drawing point to the specified point.

case closePath

Marks the end of the current subpath at the specified point.

static var curveTo: NSBezierPath.ElementType

Creates a curved line segment from the current point to the specified endpoint using two control points to define the curve.

Deprecated

case cubicCurveTo

case quadraticCurveTo

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum LineJoinStyle

Constants that specify the shape of the joins between connected segments of a stroked path.

enum LineCapStyle

Constants that specify the shape of endpoints for an open path when it is stroked.

enum WindingRule

Constants that specify the winding rule a Bézier path uses.

