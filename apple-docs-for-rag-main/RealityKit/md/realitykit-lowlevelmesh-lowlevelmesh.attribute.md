

- RealityKit
- LowLevelMesh
-  LowLevelMesh.Attribute 

Structure

# LowLevelMesh.Attribute

An object that determines how to store vertex attribute data in memory and map it to RealityKit shader attributes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Attribute
```

## Topics

### Creating a vertex attribute

init(semantic: LowLevelMesh.VertexSemantic, format: MTLVertexFormat, layoutIndex: Int, offset: Int)

Creates an attribute for a low-level mesh.

### Describing an attribute

var format: MTLVertexFormat

The format of the vertex attribute.

var offset: Int

The location of an attribute in vertex data, determined by the byte offset from the start of the vertex data.

var layoutIndex: Int

The index of the layout that contains this attribute.

var semantic: LowLevelMesh.VertexSemantic

The semantic of the vertex attribute, which describes how you want RealityKit to interpret the attribute.

## See Also

### Updatable meshes

Creating a spatial drawing app with RealityKit

Use low-level mesh and texture APIs to achieve fast updates to a person’s brush strokes by integrating RealityKit with ARKit and SwiftUI.

Creating a plane with low-level mesh

Create a low-level mesh and set its vertex positions and normals to form a plane.

class LowLevelMesh

A container for vertex data that you can use to create and update meshes using your own format.

struct Descriptor

An object that describes the data format and layout of the buffers in a low-level mesh.

struct Part

An object that describes a range of primitives to display, and their material index.

struct Layout

An object that describes a set of attributes that share a buffer index, offset, and stride.

enum VertexSemantic

Designates the intended usage of a vertex attribute.

struct PartsCollection

An object that holds a mutable collection low-level mesh parts.

