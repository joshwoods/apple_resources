

- SceneKit
-  SCNShape 

Class

# SCNShape

A geometry based on a two-dimensional path, optionally extruded to create a three-dimensional object.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
class SCNShape
```

## Overview

SceneKit creates a three-dimensional geometry by extruding a Bézier path, which extends in the x- and y-axis directions of its local coordinate space, along the z-axis by a specified amount. For example, if you create a shape with an extrusion depth of `1.0`, it extends from `-0.5` to `0.5` along the z-axis. An extrusion depth of zero creates a flat, one-sided shape—the geometry is confined to the plane whose z-coordinate is `0.0`, and viewable only from its front unless its material’s isDoubleSided property is true.

A shape geometry may contain between one and five geometry elements:

- If its extrusionDepth property is `0.0`, the shape geometry has one element corresponding to its one visible side.

- If its extrusion depth is greater than zero and its chamferRadius property is `0.0`, the shape geometry has three elements, corresponding to its front, back, and extruded sides.

- If both extrusion depth and chamfer radius are greater than zero, the text geometry can have four or five elements depending on its chamferMode property, corresponding to its front, back, extruded sides, front chamfer, and back chamfer.

SceneKit can render each element using a different material. For details, see the description of the materials property in SCNGeometry.

## Topics

### Creating a Shape

convenience init(path: UIBezierPath?, extrusionDepth: CGFloat)

Creates a shape geometry with the specified path and extrusion depth.

### Modifying a Shape

var extrusionDepth: CGFloat

The thickness of the extruded shape along the z-axis. Animatable.

var path: UIBezierPath?

The two-dimensional path forming the basis of the shape.

### Chamfering a Shape

var chamferMode: SCNChamferMode

A constant specifying which ends of the extruded shape’s profile are chamfered.

enum SCNChamferMode

Options for which edges of an extruded shape are chamfered, used by the chamferMode property.

var chamferProfile: UIBezierPath?

A path that determines the cross-sectional contour of each chamfered edge.

var chamferRadius: CGFloat

The width or depth of each chamfered edge. Animatable.

## Relationships

### Inherits From

- SCNGeometry

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- SCNAnimatable
- SCNBoundingVolume
- SCNShadable

## See Also

### Parametric Geometry

class SCNText

A geometry based on a string of text, optionally extruded to create a three-dimensional object.

