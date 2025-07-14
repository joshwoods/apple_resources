

- ARKit
-  ARMeshGeometry 

Class

# ARMeshGeometry

Mesh information stored in an efficient, array-based format.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
class ARMeshGeometry
```

## Overview

The information in this class holds the geometry data for a single anchor of the scene mesh. Each vertex in the anchor’s mesh represents one connection point. Every three-vertex combination forms a unique triangle called a *face*. Each face includes an outside-directional normal and a classification. If ARKit cannot classify a particular face, the value is `0`, –– the raw value for ARMeshClassification.none.

## Topics

### Accessing Geometry Data

var vertices: ARGeometrySource

The vertices of the mesh.

class ARGeometrySource

Mesh data in a buffer-based array.

### Getting Geometry Information

var classification: ARGeometrySource?

Classification for each face in the mesh.

enum ARMeshClassification

Enumeration of different classes of real-world objects that ARKit can identify.

var faces: ARGeometryElement

An object that contains a buffer of vertex indices of the geometry’s faces.

class ARGeometryElement

A container for index data, such as vertex indices of a face.

var normals: ARGeometrySource

Rays that define which direction is outside for each face.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Accessing the Mesh

var geometry: ARMeshGeometry

3D information about the mesh such as its shape and classifications.

