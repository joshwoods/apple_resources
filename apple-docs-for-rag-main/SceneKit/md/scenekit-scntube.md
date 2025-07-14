

- SceneKit
-  SCNTube 

Class

# SCNTube

A tube or pipe geometry—a right circular cylinder with a circular hole along its central axis.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNTube
```

## Overview

The outer surface of a tube is a cylinder. Define the size of the cylinder’s cross section in the x- and z-axis dimensions of its local coordinate space with the outerRadius property, and its extent in the y-axis dimension with the height property. A cylinder becomes a tube through the subtraction of a cylindrical volume along its central axis. Define the size of this circular hole using the tube’s innerRadius property. To position and orient a tube in a scene, attach it to the geometry property of an SCNNode object.

Control the level of detail with the radialSegmentCount and heightSegmentCount properties. A higher radial segment count creates a smoother curve for the tube’s circular inner and outer surfaces. A higher segment count in either direction produces more vertices, which can improve rendering quality for certain lighting models or custom shader effects, but at a cost to rendering performance.

A tube contains four SCNGeometryElement objects: one each for its base and top, one that wraps around its outer surface, and one that wraps around its inner surface. SceneKit can render each element using a different material. For details, see the materials property in SCNGeometry.

## Topics

### Creating a Tube

convenience init(innerRadius: CGFloat, outerRadius: CGFloat, height: CGFloat)

Creates a tube geometry with the specified inner radius, outer radius, and height.

### Adjusting a Tube’s Dimensions

var outerRadius: CGFloat

The radius of the tube’s outer circular cross section. Animatable.

var innerRadius: CGFloat

The radius of the circular hole through the tube. Animatable.

var height: CGFloat

The extent of the tube along its y-axis. Animatable.

### Adjusting Geometric Detail

var radialSegmentCount: Int

The number of subdivisions around the circumference of the tube. Animatable.

var heightSegmentCount: Int

The number of subdivisions in the inner and outer surfaces of the tube along its y-axis. Animatable.

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

class SCNPyramid

A right rectangular pyramid geometry.

class SCNSphere

A sphere (or ball or globe) geometry.

class SCNTorus

A torus, or ring-shaped geometry.

