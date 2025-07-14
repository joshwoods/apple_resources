

- SceneKit
-  SCNGeometry 

Class

# SCNGeometry

A three-dimensional shape (also called a model or mesh) that can be displayed in a scene, with attached materials that define its appearance.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNGeometry
```

## Overview

In SceneKit, geometries attached to SCNNode objects form the visible elements of a scene, and SCNMaterial objects attached to a geometry determine its appearance.

### Working with Geometry Objects

You control a geometry’s appearance in a scene with nodes and materials. A geometry object provides only the form of a visible object rendered by SceneKit. You specify color and texture for a geometry’s surface, control how it responds to light, and add special effects by attaching materials (for details, see the methods in Managing a Geometry’s Materials). You position and orient a geometry in a scene by attaching it to an SCNNode object. Multiple nodes can reference the same geometry object, allowing it to appear at different positions in a scene.

You can easily copy geometries and change their materials. A geometry object manages the association between immutable vertex data and a mutable assignment of materials. To make a geometry appear more than once in the same scene with a different set of materials, use its inherited copy() method. The copy shares the underlying vertex data of the original, but can be assigned materials independently. You can thus make many copies of a geometry without incurring a significant cost to rendering performance.

You can animate a geometry object. The vertex data associated with a geometry is immutable, but SceneKit provides several ways to animate geometry. You can use a SCNMorpher or SCNSkinner object to deform a geometry’s surface, or run animations created in an external 3D authoring tool and loaded from a scene file. You can also use methods in the SCNShadable protocol to add custom GLSL shader programs that alter SceneKit’s rendering of a geometry.

### Obtaining a Geometry Object

SceneKit provides several ways to introduce geometry objects to your app:

| Action | For further information |
|----|----|
| Load from a scene file created using external 3D authoring tools | SCNScene, SCNSceneSource |
| Use and customize SceneKit’s built-in primitive shapes | SCNPlane, SCNBox, SCNSphere, SCNPyramid, SCNCone, SCNCylinder, SCNCapsule, SCNTube, and SCNTorus |
| Create 3D geometry from 2D text or Bézier curves | SCNText, SCNShape |
| Create a custom geometry from vertex data | SCNGeometrySource, SCNGeometryElement, init(sources:elements:), Managing Geometry Data |

## Topics

### Creating a Geometry Object

convenience init(sources: [SCNGeometrySource], elements: [SCNGeometryElement]?)

Creates a new geometry built from the specified geometry sources and elements.

### Managing Geometry Attributes

var name: String?

A name associated with the geometry object.

protocol SCNBoundingVolume

Methods common to the SCNNode and SCNGeometry classes for measuring location and size.

### Managing a Geometry’s Materials

var materials: [SCNMaterial]

An array of SCNMaterial objects that determine the geometry’s appearance when rendered.

var firstMaterial: SCNMaterial?

The first material attached to the geometry.

func material(named: String) -> SCNMaterial?

Returns the first material attached to the geometry with the specified name.

func insertMaterial(SCNMaterial, at: Int)

Attaches a material to the geometry at the specified index.

func removeMaterial(at: Int)

Removes a material attached to the geometry.

func replaceMaterial(at: Int, with: SCNMaterial)

Replaces a material attached to the geometry with another.

### Managing Geometry Data

var elements: [SCNGeometryElement]

An array of geometry elements that describe the geometry’s shape.

var sources: [SCNGeometrySource]

An array of geometry sources that provide vertex data for the geometry.

var elementCount: Int

The number of geometry elements in the geometry.

func element(at: Int) -> SCNGeometryElement

Returns the geometry element at a specified index.

func sources(for: SCNGeometrySource.Semantic) -> [SCNGeometrySource]

Returns the geometry sources for a specified semantic.

### Optimizing Level of Detail

var levelsOfDetail: [SCNLevelOfDetail]?

An array of SCNLevelOfDetail objects for managing the geometry’s appearance when viewed from far away.

class SCNLevelOfDetail

An alternate resolution for a geometry that SceneKit automatically substitutes to improve rendering performance.

### Smoothing and Subdividing Geometry

var subdivisionLevel: Int

The number of subdivisions SceneKit uses to smooth the geometry’s surface at render time.

var edgeCreasesElement: SCNGeometryElement?

The geometry element identifying which edges of the geometry’s surface should remain sharp after subdivision.

var edgeCreasesSource: SCNGeometrySource?

The geometry source specifying the smoothness or sharpness of edges after surface subdivision.

var wantsAdaptiveSubdivision: Bool

### Managing Tessellation

var tessellator: SCNGeometryTessellator?

class SCNGeometryTessellator

### Initializers

convenience init(sources: [SCNGeometrySource], elements: [SCNGeometryElement]?, sourceChannels: [NSNumber]?)

### Instance Properties

var geometrySourceChannels: [NSNumber]?

## Relationships

### Inherits From

- NSObject

### Inherited By

- SCNBox
- SCNCapsule
- SCNCone
- SCNCylinder
- SCNFloor
- SCNPlane
- SCNPyramid
- SCNShape
- SCNSphere
- SCNText
- SCNTorus
- SCNTube

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

### Geometry

class SCNGeometrySource

A container for vertex data forming part of the definition for a three-dimensional object, or geometry.

class SCNGeometryElement

A container for index data describing how vertices connect to define a three-dimensional object, or geometry.

Built-in Geometry Types

Basic shapes—such as spheres, boxes, and planes—and features for generating 3D objects from 2D text and Bézier curves.

