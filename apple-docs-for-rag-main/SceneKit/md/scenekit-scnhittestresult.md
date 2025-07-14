

- SceneKit
-  SCNHitTestResult 

Class

# SCNHitTestResult

Information about the result of a scene-space or view-space search for scene elements.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNHitTestResult
```

## Overview

Hit-testing is the process of finding elements of a scene located at a specified point, or along a specified line segment (or *ray*). An SCNHitTestResult object provides details about one result from a hit-test search. There are three ways to perform a hit-test search. Use the hitTest(_:options:) method of an SCNView object (or other scene renderer), the hitTestWithSegment(from:to:options:) method of a node, or the rayTestWithSegment(from:to:options:) method of your scene’s physics world.

When you perform a hit-test search, SceneKit looks for SCNGeometry objects along the ray you specify. For each intersection between the ray and and a geometry, SceneKit creates a hit-test result to provide information about both the SCNNode object containing the geometry and the location of the intersection on the geometry’s surface.

## Topics

### Retrieving Information About a Hit-Test Result

var node: SCNNode

The node whose geometry intersects the search ray.

var geometryIndex: Int

The index of the geometry element whose surface the search ray intersects.

var faceIndex: Int

The index of the primitive in the geometry element intersected by the search ray.

var localCoordinates: SCNVector3

The point of intersection between the geometry and the search ray, in the local coordinate system of the node containing the geometry.

var worldCoordinates: SCNVector3

The point of intersection between the geometry and the search ray, in the scene’s world coordinate system.

var localNormal: SCNVector3

The surface normal vector at the point of intersection, in the local coordinate system of the node containing the geometry intersected by the search ray.

var worldNormal: SCNVector3

The surface normal vector at the point of intersection, in the scene’s world coordinate system.

var modelTransform: SCNMatrix4

The world transform matrix of the node containing the intersection.

func textureCoordinates(withMappingChannel: Int) -> CGPoint

Returns the texture coordinates at the point of intersection for the specified texture mapping channel.

### Instance Properties

var boneNode: SCNNode?

var simdLocalCoordinates: simd_float3

var simdLocalNormal: simd_float3

var simdModelTransform: simd_float4x4

var simdWorldCoordinates: simd_float3

var simdWorldNormal: simd_float3

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Display and Interactivity

protocol SCNSceneRenderer

Methods and properties common to the SCNView, SCNLayer, and SCNRenderer classes.

protocol SCNSceneRendererDelegate

Methods your app can implement to participate in SceneKit’s animation loop or perform additional rendering.

class SCNLayer

A Core Animation layer that renders a SceneKit scene as its content.

Deprecated

class SCNRenderer

A renderer for displaying a SceneKit scene in an existing Metal workflow or OpenGL context.

