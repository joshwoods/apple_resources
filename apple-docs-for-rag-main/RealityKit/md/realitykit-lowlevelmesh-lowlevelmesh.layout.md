

- RealityKit
- LowLevelMesh
-  LowLevelMesh.Layout 

Structure

# LowLevelMesh.Layout

An object that describes a set of attributes that share a buffer index, offset, and stride.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Layout
```

## Overview

Applications typically express their types using contiguous or interleaved (strided) memory.

If you interleave your data (meaning that you represent it with a structure), use one `Layout` object where bufferStride is equal to `MemoryLayout.stride()`.

If you store your attributes separately, use one `Layout` per attribute.

## Topics

### Creating a low-level mesh layout

init(bufferIndex: Int, bufferOffset: Int, bufferStride: Int)

### Describing a low-level mesh layout

var bufferIndex: Int

The index of the buffer to use for this layout.

var bufferOffset: Int

The byte offset into the buffer for the first byte of this layout.

var bufferStride: Int

The distance, in bytes, between consecutive vertices for attributes using this layout.

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

struct Attribute

An object that determines how to store vertex attribute data in memory and map it to RealityKit shader attributes.

enum VertexSemantic

Designates the intended usage of a vertex attribute.

struct PartsCollection

An object that holds a mutable collection low-level mesh parts.

