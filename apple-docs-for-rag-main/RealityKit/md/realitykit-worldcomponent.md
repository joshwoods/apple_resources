

- RealityKit
-  WorldComponent 

Structure

# WorldComponent

A component that defines a portal world.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct WorldComponent
```

## Overview

This component separates an entity and its descendants from the default world, allowing it to only be visible through a portal.

Use a PortalComponent and point its targetEntity to this entity to render this world.

See PortalComponent for information about example usage, clipping, crossing, and lighting.

## Topics

### Initializers

init()

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Portals

struct PortalMaterial

A material that makes the mesh part a portal to a different world.

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TriangleFillMode

An alias for the triangle fill mode object that’s appropriate for this material class.

struct PortalComponent

A component that turns mesh surfaces into portals to a different world.

struct PortalCrossingComponent

A component that allows entities to cross portal boundaries.

