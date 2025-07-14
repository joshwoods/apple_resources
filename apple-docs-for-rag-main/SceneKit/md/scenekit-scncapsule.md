

- SceneKit
-  SCNCapsule 

Class

# SCNCapsule

A right circular cylinder geometry whose ends are capped with hemispheres.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNCapsule
```

## Overview

Define the size of the two hemispheres forming the ends of a capsule with the capRadius property. Because the cylindrical body of the capsule stretches between the its two hemispherical ends, its circular cross section in the x- and z-axis dimensions has the same radius. Define the capsule’s extent in the z-axis dimension of its local coordinate space with the height property. To change the orientation of a capsule, adjust the transform property of the node containing the capsule geometry.

Control the level of detail with the heightSegmentCount, capSegmentCount, and height properties. Higher radial and cap segment counts create smoother curves for the cylinder’s circular sides and hemispherical ends. A higher segment count in any direction produces more vertices, which can improve rendering quality for certain lighting models or custom shader effects, but at a cost to rendering performance.

## Topics

### Creating a Capsule

convenience init(capRadius: CGFloat, height: CGFloat)

Creates a capsule geometry with the specified radius and height.

### Adjusting a Capsule’s Dimensions

var capRadius: CGFloat

The radius both of the capsule’s circular center cross section and of its hemispherical ends. Animatable.

var height: CGFloat

The extent of the capsule along its y-axis. Animatable.

### Adjusting Geometric Detail

var radialSegmentCount: Int

The number of subdivisions around the lateral circumference of the capsule. Animatable.

var capSegmentCount: Int

The number of subdivisions in the height of each hemispherical end of the capsule. Animatable.

var heightSegmentCount: Int

The number of subdivisions in the sides of the capsule along its y-axis. Animatable.

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

