

- RealityKit
- MeshResource
-  MeshResource.Instance 

Structure

# MeshResource.Instance

An object that transforms a model to a location.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Instance
```

## Topics

### Initializers

init(id: String, model: String, at: simd_float4x4?)

### Instance Properties

var id: String

The stable identity of the entity associated with this instance.

var model: String

Name of the model to instance.

var transform: simd_float4x4

Transform for the instance.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable

## See Also

### Mesh resource data

struct Contents

Value of the contents of the resource.

struct Model

A model consists of a list of parts.

struct Part

A part of a model consisting of a single material.

