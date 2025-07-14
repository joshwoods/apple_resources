

- ARKit
-  ARPlaneAnchor 

Class

# ARPlaneAnchor

An anchor for a 2D planar surface that ARKit detects in the physical environment.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARPlaneAnchor
```

## Overview

When you enable planeDetection in a world tracking session, ARKit notifies your app of all the surfaces it observes using the device’s back camera. ARKit calls your delegate’s session(_:didAdd:) with an ARPlaneAnchor for each unique surface. Each plane anchor provides details about the surface, like its real-world position and shape.

The width and length of a plane (the planeExtent) span the xz-plane of an ARPlaneAnchor instance’s local coordinate system. The y-axis of the plane anchor is the plane’s normal vector.

## Topics

### Orientation

var alignment: ARPlaneAnchor.Alignment

The general orientation of the detected plane with respect to gravity.

enum Alignment

The kinds of alignment — horizontal or vertical — that a plane anchor can have.

### Geometry

var geometry: ARPlaneGeometry

A coarse triangle mesh representing the general shape of the detected plane.

class ARPlaneGeometry

A 3D mesh describing the shape of a detected plane in world-tracking AR sessions.

class ARSCNPlaneGeometry

A SceneKit representation of the 2D shape of a plane, for use with plane detection results in an AR session.

### Dimensions

var center: simd_float3

The center point of the plane relative to its anchor position.

var planeExtent: ARPlaneExtent

The estimated width, length, and y-axis rotation of the detected plane.

class ARPlaneExtent

The size and y-axis rotation of a detected plane.

var extent: simd_float3

The estimated width and length of the detected plane.

Deprecated

### Classifying a Plane

class var isClassificationSupported: Bool

A Boolean value that indicates whether plane classification is available on the current device.

var classification: ARPlaneAnchor.Classification

A general characterization of what kind of real-world surface the plane anchor represents.

enum Classification

Possible characterizations of real-world surfaces represented by plane anchors.

## Relationships

### Inherits From

- ARAnchor

### Conforms To

- ARAnchorCopying
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Surface Detection

Tracking and visualizing planes

Detect surfaces in the physical environment and visualize their shape and location in 3D space.

class ARMeshAnchor

An anchor for a physical object that ARKit detects and recreates virtually using a polygonal mesh.

