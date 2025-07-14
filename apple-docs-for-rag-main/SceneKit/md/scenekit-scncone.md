

- SceneKit
-  SCNCone 

Class

# SCNCone

A right circular cone or frustum geometry.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNCone
```

## Overview

A cone defines the surface of a solid whose base is a circle and whose side surface tapers to a point centered above its base. A frustum also has a circular base and tapered sides but has a circular top, similar to a cone cut off below its apex.

Define the size of the cone’s base in the x- and z-axis dimensions of its local coordinate space with its bottomRadius property, and its extent in the y-axis dimension with its height property. Create a cone that tapers to a point by setting its topRadius property to zero, or a frustum that tapers (or expands) to a circular top by setting the topRadius property to a different value.

To position and orient a cone in a scene, attach it to the geometry property of an SCNNode object.

Control the level of detail with the radialSegmentCount and heightSegmentCount properties. A higher radial segment count creates a smoother curve for the cone’s circular sides. A higher segment count in either direction produces more vertices, which can improve rendering quality for certain lighting models or custom shader effects, but at a cost to rendering performance.

A cone geometry may contain two or three SCNGeometryElement objects, corresponding to its outer surface, its base and its top (or base only or top only, if the topRadius or bottomRadius property is zero). SceneKit can render each element using a different material. For details, see the materials property in SCNGeometry.

## Topics

### Creating a Cone

convenience init(topRadius: CGFloat, bottomRadius: CGFloat, height: CGFloat)

Creates a cone geometry with the given top radius, bottom radius, and height.

### Adjusting a Cone’s Dimensions

var topRadius: CGFloat

The radius of the cone’s circular top. Animatable.

var bottomRadius: CGFloat

The radius of the cone’s circular base. Animatable.

var height: CGFloat

The extent of the cylinder along its y-axis. Animatable.

### Adjusting Geometric Detail

var radialSegmentCount: Int

The number of subdivisions around the circumference of the cone. Animatable.

var heightSegmentCount: Int

The number of subdivisions in the sides of the cone along its y-axis. Animatable.

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

