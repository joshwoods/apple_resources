

- SceneKit
-  SCNTorus 

Class

# SCNTorus

A torus, or ring-shaped geometry.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNTorus
```

## Overview

A torus is mathematically defined as a surface of revolution formed by revolving a circle around a coplanar axis. It is the product of two circles: a large ring and a pipe that encircles the ring. SceneKit uses these terms to define the dimensions of a torus geometry in its local coordinate space. The torus’ ringRadius property defines a circle in the x- and z-axis dimensions, centered at the origin, and its pipeRadius property defines the width of the surface encircling the ring. To change the orientation of a torus, adjust the transform property of the node containing the torus geometry.

Control the level of detail with the ringSegmentCount and pipeSegmentCount properties. Higher segment counts produce more vertices and a more smoothly curved surface, which can improve rendering quality at a cost to rendering performance.

## Topics

### Creating a Torus

convenience init(ringRadius: CGFloat, pipeRadius: CGFloat)

Creates a torus geometry with the specified ring radius and pipe radius.

### Adjusting a Torus’ Dimensions

var ringRadius: CGFloat

The major radius of the torus, defining a circle in the x- and z-axis dimensions. Animatable.

var pipeRadius: CGFloat

The minor radius of the torus, defining the pipe that encircles the torus ring. Animatable.

### Configuring Torus Properties

var ringSegmentCount: Int

The number of subdivisions around the torus ring. Animatable.

var pipeSegmentCount: Int

The number of subdivisions around the torus pipe. Animatable.

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

class SCNTube

A tube or pipe geometry—a right circular cylinder with a circular hole along its central axis.

