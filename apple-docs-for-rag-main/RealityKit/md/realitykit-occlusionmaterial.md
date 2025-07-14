

- RealityKit
-  OcclusionMaterial 

Structure

# OcclusionMaterial

An invisible material that hides objects rendered behind it.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct OcclusionMaterial
```

## Overview

Add an `OcclusionMaterial` to a model by setting it as one of the materials in a ModelComponent.

```
let model = ModelComponent(
    mesh: .generateBox(size: 1),
    materials: [OcclusionMaterial()]
)
smallBoxEntity.components.set(model)
```

For example, on the left is a case of two cubes, the larger red cube is slightly further from the camera and has a simple material. The slightly smaller and closer cube has no material in the left image and an occlusion material on the right image.

| No material | Occlusion material |
|----|----|
|  |  |

## Topics

### Creating an occlusion material

init(receivesDynamicLighting: Bool)

Creates an occlusion material.

init()

### Receiving dynamic lighting

let receivesDynamicLighting: Bool

A Boolean that indicates whether the occlusion material receives dynamic lighting.

### Setting depth testing properties

var readsDepth: Bool

A boolean value that determines whether this material performs the depth test by reading RealityKit’s depth buffer.

### Instance Properties

var faceCulling: OcclusionMaterial.FaceCulling

A process in which the system specifies polygons to remove before rendering a mesh using this material.

### Type Aliases

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

### Default Implementations

Material Implementations

## Relationships

### Conforms To

- Material
- Sendable

## See Also

### Object occlusion

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

