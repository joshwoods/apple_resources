

- RealityKit
- LowLevelMesh
-  LowLevelMesh.VertexSemantic 

Enumeration

# LowLevelMesh.VertexSemantic

Designates the intended usage of a vertex attribute.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum VertexSemantic
```

## Overview

RealityKit consults the vertex semantic when interpreting the data in your LowLevelMesh. For example, an attribute with the semantic value of LowLevelMesh.VertexSemantic.position determines the position of a vertex.

## Topics

### Specifying intended use

case bitangent

The semantic for surface bitangent vector data.

case color

The semantic for per-vertex color data.

case normal

The semantic for surface normal data.

case position

The semantic for vertex position data.

case tangent

The semantic for surface tangent vector data.

case unspecified

The semantic that doesn’t specify the role of the vertex.

case uv0

The semantic for the first UV channel, also known as UV0.

case uv1

The semantic for the second UV channel, also known as UV1.

case uv2

The semantic for the third UV channel, also known as UV2.

case uv3

The semantic for the fourth UV channel, also known as UV3.

case uv4

The semantic for the fifth UV channel, also known as UV4.

case uv5

The semantic for the sixth UV channel, also known as UV5.

case uv6

The semantic for the seventh UV channel, also known as UV6.

case uv7

The semantic for the eighth UV channel, also known as UV7.

### Comparing enumeration values

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func == (LowLevelMesh.VertexSemantic, LowLevelMesh.VertexSemantic) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

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

struct Attribute

An object that determines how to store vertex attribute data in memory and map it to RealityKit shader attributes.

struct PartsCollection

An object that holds a mutable collection low-level mesh parts.

