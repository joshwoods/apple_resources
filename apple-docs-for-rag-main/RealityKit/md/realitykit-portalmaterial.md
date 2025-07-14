

- RealityKit
-  PortalMaterial 

Structure

# PortalMaterial

A material that makes the mesh part a portal to a different world.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct PortalMaterial
```

## Overview

You use a `PortalMaterial` with PortalComponent and WorldComponent to enable portal features.

You can set this material on individual mesh parts. For example, create a box with generateBox(width:height:depth:cornerRadius:splitFaces:). It can have some faces using PhysicallyBasedMaterial and some faces using `PortalMaterial`.

```
let portal = Entity()
// When you set `splitFaces` to `true`, each face takes up a different material slot.
let cyanMaterial = SimpleMaterial(color: .cyan, isMetallic: false)
portal.components.set(ModelComponent(
    mesh: .generateBox(width: 0.5, height: 0.5, depth: 0.5, splitFaces: true),
    materials: [PortalMaterial(),
                cyanMaterial,
                cyanMaterial,
                cyanMaterial,
                cyanMaterial,
                cyanMaterial]
))
// Because the box has `0.5 x 0.5 x 0.5` dimensions,
// offset the portal plane on the z-axis by 0.25 so that
// it's at the front of the cube.
// Make sure it faces toward the positive z-direction.
portal.components.set(PortalComponent(
    target: world,
    clippingMode: .disabled,
    crossingMode: .plane(PortalComponent.Plane(position: [0, 0, 0.25], normal: [0, 0, 1]))
))
```

RealityKit treats each mesh part with a `PortalMaterial` as a different portal, even if they are pointing to the same world. Beware of the performance impact of this usage.

See PortalComponent for example usage.

## Topics

### Initializers

init()

### Instance Properties

var faceCulling: PortalMaterial.FaceCulling

A process in which the system specifies polygons to remove before rendering a mesh using this material.

var triangleFillMode: PortalMaterial.TriangleFillMode

The object that controls how RealityKit draws triangles.

### Type Aliases

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TriangleFillMode

An alias for the triangle fill mode object that’s appropriate for this material class.

### Default Implementations

Material Implementations

## Relationships

### Conforms To

- Material
- Sendable

## See Also

### Portals

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TriangleFillMode

An alias for the triangle fill mode object that’s appropriate for this material class.

struct PortalComponent

A component that turns mesh surfaces into portals to a different world.

struct WorldComponent

A component that defines a portal world.

struct PortalCrossingComponent

A component that allows entities to cross portal boundaries.

