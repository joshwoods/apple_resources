

- RealityKit
- MeshResource
-  MeshResource.Model 

Structure

# MeshResource.Model

A model consists of a list of parts.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Model
```

## Topics

### Initializers

init(id: String, descriptors: [MeshDescriptor]) throws

init(id: String, parts: [MeshResource.Part])

### Instance Properties

var id: String

The stable identity of the entity associated with this instance.

var parts: MeshPartCollection

Table of parts composing this mesh.

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

struct Instance

An object that transforms a model to a location.

struct Part

A part of a model consisting of a single material.

