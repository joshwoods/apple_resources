

- SceneKit
-  SCNBox 

Class

# SCNBox

A six-sided polyhedron geometry whose faces are all rectangles, optionally with rounded edges and corners.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNBox
```

## Overview

Define the shape of the box in the x-, y-, and z-axis dimensions of its local coordinate space by setting its width, height, and length properties. Add rounded edges and corners to a box with its chamferRadius property. To position and orient a box in a scene, attach it to the geometry property of an SCNNode object.

Control the level of detail with the widthSegmentCount, heightSegmentCount, lengthSegmentCount, and chamferSegmentCount properties. A higher segment count produces more vertices, which can improve rendering quality for certain lighting models or custom shader effects, but at a cost to rendering performance.

You can assign up to six SCNMaterial instances to a box—one for each side—with its materials property. The SCNBox class automatically creates SCNGeometryElement objects as needed to handle the number of materials.

## Topics

### Creating a Box

convenience init(width: CGFloat, height: CGFloat, length: CGFloat, chamferRadius: CGFloat)

Creates a box geometry with the specified width, height, length, and chamfer radius.

### Adjusting a Box’s Dimensions

var width: CGFloat

The extent of the box along its x-axis. Animatable.

var height: CGFloat

The extent of the box along its y-axis. Animatable.

var length: CGFloat

The extent of the box along its z-axis. Animatable.

### Configuring Box Properties

var widthSegmentCount: Int

The number of subdivisions in each face of the box along its x-axis. Animatable.

var heightSegmentCount: Int

The number of subdivisions in each face of the box along its y-axis. Animatable.

var lengthSegmentCount: Int

The number of subdivisions in each face of the box along its z-axis. Animatable.

### Adding Rounded Edges and Corners

var chamferRadius: CGFloat

The radius of curvature for the edges and corners of the box. Animatable.

var chamferSegmentCount: Int

The number of line segments used to create each rounded edge of the box. Animatable.

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

class SCNCapsule

A right circular cylinder geometry whose ends are capped with hemispheres.

class SCNCone

A right circular cone or frustum geometry.

class SCNCylinder

A right circular cylinder geometry.

class SCNPlane

A rectangular, one-sided plane geometry of specified width and height.

class SCNPyramid

A right rectangular pyramid geometry.

class SCNSphere

A sphere (or ball or globe) geometry.

class SCNTorus

A torus, or ring-shaped geometry.

class SCNTube

A tube or pipe geometry—a right circular cylinder with a circular hole along its central axis.

