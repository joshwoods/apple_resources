

- SceneKit
-  SCNCylinder 

Class

# SCNCylinder

A right circular cylinder geometry.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNCylinder
```

## Overview

A cylinder defines the surface of a solid whose every cross section along a linear axis is a circle of equal size. Define the size of the cylinder’s cross section in the x- and z-axis dimensions of its local coordinate space with the radius property, and its extent in the y-axis dimension with the height property. To position and orient a cylinder in a scene, attach it to the geometry property of an SCNNode object.

Control the level of detail with the radialSegmentCount and heightSegmentCount properties. A higher radial segment count creates a smoother curve for the cylinder’s circular sides. A higher segment count in either direction produces more vertices, which can improve rendering quality for certain lighting models or custom shader effects, but at a cost to rendering performance.

A cylinder contains three SCNGeometryElement objects: one each for its base and top, and one that wraps around its sides. SceneKit can render each element using a different material. For details, see the materials property in SCNGeometry.

## Topics

### Creating a Cylinder

convenience init(radius: CGFloat, height: CGFloat)

Creates a cylinder geometry with the specified radius and height.

### Adjusting a Cylinder’s Dimensions

var radius: CGFloat

The radius of the cylinder’s circular cross section. Animatable.

var height: CGFloat

The extent of the cylinder along its y-axis. Animatable.

### Adjusting Geometric Detail

var radialSegmentCount: Int

The number of subdivisions around the circumference of the cylinder. Animatable.

var heightSegmentCount: Int

The number of subdivisions in the sides of the cylinder along its y-axis. Animatable.

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

