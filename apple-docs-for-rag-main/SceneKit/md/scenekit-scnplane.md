

- SceneKit
-  SCNPlane 

Class

# SCNPlane

A rectangular, one-sided plane geometry of specified width and height.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNPlane
```

## Overview

A plane defines a flat surface in the x- and y-axis dimensions of its local coordinate space according to its width and height properties. To orient a plane differently, adjust the transform property of the node containing the plane geometry. You can create a rounded rectangular plane using the cornerRadius property.

The surface is one-sided. Its surface normal vectors point in the positive z-axis direction of its local coordinate space, so it is only visible from that direction by default. To render both sides of a plane, either set the isDoubleSided property of its material to true or create two plane geometries and orient them back to back.

Control the level of detail with the widthSegmentCount, heightSegmentCount, and cornerSegmentCount properties. A higher segment count produces more vertices, which can improve rendering quality for certain lighting models or custom shader effects, but at a cost to rendering performance.

## Topics

### Creating a Plane

convenience init(width: CGFloat, height: CGFloat)

Creates a plane geometry with the specified width and height.

### Adjusting a Plane’s Dimensions

var width: CGFloat

The extent of the plane along its horizontal axis. Animatable.

var height: CGFloat

The extent of the plane along its vertical axis. Animatable.

### Adjusting Geometric Detail

var widthSegmentCount: Int

The number of subdivisions in the plane’s surface along its horizontal axis. Animatable.

var heightSegmentCount: Int

The number of subdivisions in the plane’s surface along its vertical axis. Animatable.

### Adding Rounded Corners

var cornerRadius: CGFloat

The radius of curvature for the plane’s corners. Animatable.

var cornerSegmentCount: Int

The number of line segments used to create each rounded corner of the plane. Animatable.

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

### Basic Shapes

class SCNFloor

A plane that can optionally display a reflection of the scene above it.

class SCNBox

A six-sided polyhedron geometry whose faces are all rectangles, optionally with rounded edges and corners.

class SCNCapsule

A right circular cylinder geometry whose ends are capped with hemispheres.

class SCNCone

A right circular cone or frustum geometry.

class SCNCylinder

A right circular cylinder geometry.

class SCNPyramid

A right rectangular pyramid geometry.

class SCNSphere

A sphere (or ball or globe) geometry.

class SCNTorus

A torus, or ring-shaped geometry.

class SCNTube

A tube or pipe geometry—a right circular cylinder with a circular hole along its central axis.

