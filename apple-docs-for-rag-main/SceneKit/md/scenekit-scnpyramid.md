

- SceneKit
-  SCNPyramid 

Class

# SCNPyramid

A right rectangular pyramid geometry.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNPyramid
```

## Overview

A pyramid defines the surface of a solid whose base is a rectangle, and whose four triangular side faces converge at a point centered above its base. Define the shape of the pyramid’s base in the x- and z-axis dimensions of its local coordinate space with the width and length properties, and its extent in the y-axis dimension with the height property. To position and orient a pyramid in a scene, attach it to the geometry property of an SCNNode object.

Control the level of detail with the widthSegmentCount, lengthSegmentCount, and heightSegmentCount properties. A higher segment count produces more vertices, which can improve rendering quality for certain lighting models or custom shader effects, but at a cost to rendering performance.

A pyramid contains five SCNGeometryElement objects, corresponding to its base and each of its four sides. SceneKit can render each element using a different material. For details, see the materials property in SCNGeometry.

## Topics

### Creating a Pyramid

convenience init(width: CGFloat, height: CGFloat, length: CGFloat)

Creates a pyramid geometry with the specified width, height, and length.

### Adjusting a Pyramid’s Dimensions

var width: CGFloat

The extent of the pyramid along its x-axis. Animatable.

var height: CGFloat

The extent of the pyramid along its y-axis. Animatable.

var length: CGFloat

The extent of the pyramid along its z-axis. Animatable.

### Adjusting Geometric Detail

var widthSegmentCount: Int

The number of subdivisions in each face of the pyramid along its x-axis. Animatable.

var heightSegmentCount: Int

The number of subdivisions in each face of the pyramid along its y-axis. Animatable.

var lengthSegmentCount: Int

The number of subdivisions in each face of the pyramid along its z-axis. Animatable.

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

class SCNPlane

A rectangular, one-sided plane geometry of specified width and height.

class SCNSphere

A sphere (or ball or globe) geometry.

class SCNTorus

A torus, or ring-shaped geometry.

class SCNTube

A tube or pipe geometry—a right circular cylinder with a circular hole along its central axis.

