

- SceneKit
-  SCNFloor 

Class

# SCNFloor

A plane that can optionally display a reflection of the scene above it.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNFloor
```

## Overview

By default, a floor extends infinitely in the x- and z-axis dimensions of its local coordinate space, and is located in the plane whose y-coordinate is zero. To position and orient a floor in a scene, attach it to the geometry property of an SCNNode object. Often, you use a floor to provide a background for a scene.

If a floor’s reflectivity property is greater than zero, SceneKit automatically renders reflections for all geometries above it. Optionally, you can add an opacity gradient so that reflections of scene contents closer to the floor appear more clearly than those of scene contents further from it. You control the floor’s reflectivity using the properties listed in Adding Reflections to a Floor.

## Topics

### Adding Reflections to a Floor

var reflectivity: CGFloat

The intensity of the scene’s reflection on the floor. Animatable.

var reflectionFalloffEnd: CGFloat

The distance from the floor at which scene contents are no longer reflected. Animatable.

var reflectionFalloffStart: CGFloat

The distance from the floor at which scene contents are reflected at full intensity. Animatable.

var reflectionResolutionScaleFactor: CGFloat

The resolution scale factor of the offscreen buffer that SceneKit uses to render reflections.

var reflectionCategoryBitMask: Int

A mask that defines which categories of other objects show reflections on the floor.

### Adjusting a Floor’s Size

var width: CGFloat

The extent of the floor along its x-axis. Animatable.

var length: CGFloat

The extent of the floor along its z-axis. Animatable.

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

class SCNTube

A tube or pipe geometry—a right circular cylinder with a circular hole along its central axis.

