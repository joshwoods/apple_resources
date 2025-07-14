

- RealityKit
-  PortalCrossingComponent 

Structure

# PortalCrossingComponent

A component that allows entities to cross portal boundaries.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct PortalCrossingComponent
```

## Overview

You use this with PortalComponent.CrossingMode to enable portal crossing features.

When you set this on an entity, this component defines whether the entity is capable of crossing the portal boundary.

Entities without this component, entities where isEnabled is `false`, and entities without a containing entity that specifies inherited portal crossing, aren’t able to cross portals.

See PortalComponent for detailed usage.

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

struct WorldComponent

A component that defines a portal world.

