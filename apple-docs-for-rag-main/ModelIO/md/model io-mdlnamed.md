

- Model I/O
-  MDLNamed 

Protocol

# MDLNamed

The common interface for Model I/O objects that expose a human-readable name.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol MDLNamed
```

## Overview

The name property defined by this protocol is adopted by many classes in Model I/O. You can use this property to assign descriptive names to objects such as meshes, materials, cameras, and scattering functions to better keep track of the objects in your app. When you load objects from or export objects to a file using the MDLAsset class, this property corresponds to the names and labels for objects that appear in popular 3D authoring tools.

## Topics

### Naming an Object

var name: String

A descriptive name for the object.

**Required**

## Relationships

### Conforming Types

- MDLAreaLight
- MDLCamera
- MDLCheckerboardTexture
- MDLColorSwatchTexture
- MDLLight
- MDLLightProbe
- MDLMaterial
- MDLMaterialProperty
- MDLMaterialPropertyConnection
- MDLMaterialPropertyGraph
- MDLMaterialPropertyNode
- MDLMesh
- MDLNoiseTexture
- MDLNormalMapTexture
- MDLObject
- MDLPackedJointAnimation
- MDLPhotometricLight
- MDLPhysicallyPlausibleLight
- MDLPhysicallyPlausibleScatteringFunction
- MDLScatteringFunction
- MDLSkeleton
- MDLSkyCubeTexture
- MDLStereoscopicCamera
- MDLSubmesh
- MDLTexture
- MDLURLTexture
- MDLVoxelArray

## See Also

### 3D Asset Basics

class MDLAsset

An indexed container for 3D objects and associated information, such as transform hierarchies, meshes, cameras, and lights.

class MDLObject

The base class for objects that are part of a 3D asset, including meshes, cameras, and lights.

class MDLTransform

A description of the local coordinate space transformations for a 3D object.

class MDLMesh

A container for vertex buffer data to be used in rendering a 3D object.

class MDLSubmesh

A container for index buffer data and material information to be used in rendering all or part of a 3D object.

class MDLSubmeshTopology

A description of how a submesh’s index buffer data is arranged and how that arrangement should be used to produce the submesh’s intended 3D shape.

