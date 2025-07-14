

- RealityKit
-  PortalComponent 

Structure

# PortalComponent

A component that turns mesh surfaces into portals to a different world.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct PortalComponent
```

## Overview

A RealityKit portal defines a way to look into a different, immersive world. You define an entity as a portal when it also has a ModelComponent that contains a mesh part with PortalMaterial.

To create a portal, set its targetEntity property to an entity with a WorldComponent. Entities under that world only render within the portal.

```
let world = Entity()
world.components.set(WorldComponent())

let portal = Entity()
portal.components.set(
   ModelComponent(
       mesh: .generatePlane(width: 0.5, height: 0.5, cornerRadius: 0.1),
       materials: [PortalMaterial()]
   )
)
portal.components.set(PortalComponent(target: world))

content.add(world)
content.add(portal)
```

### Clipping and Crossing

You can enable clipping by configuring clippingMode to something other than PortalComponent.ClippingMode.disabled. For example, you can use PortalComponent.ClippingMode.plane(_:). This ensures that the contents of the portal world don’t render beyond the portal boundary, causing depth confusion.

Entities inside the portal world with a PortalCrossingComponent can freely cross in and out of the portal boundary in any of the following platforms:

- iOS 18 and later

- macOS 15 and later

- visionOS 2 and later

You can enable the crossing feature by configuring crossingMode to something other than PortalComponent.CrossingMode.disabled. Such as PortalComponent.CrossingMode.plane(_:).

```
let world = Entity()
world.components.set(WorldComponent())

// Create an entity that doesn't cross beyond the portal bounds.
let notCrossing = Entity()

// Create an entity that crosses beyond the portal bounds.
let willCross = Entity()
willCross.components.set(PortalCrossingComponent())

world.addChild(notCrossing)
world.addChild(willCross)

// Set up a crossable portal, without a near clip.
let portal = Entity()
portal.components.set(
   ModelComponent(
       mesh: .generatePlane(width: 0.5, height: 0.5, cornerRadius: 0.1),
       materials: [PortalMaterial()]
   )
)
var portalComp = PortalComponent(target: world)
portalComp.clippingMode = .plane(.positiveZ)
portalComp.crossingMode = .plane(.positiveZ)
portal.components.set(portalComp)

content.add(world)
content.add(portal)
```

The spaceships below have a PortalCrossingComponent.

 Video with custom controls. 

 Content description: Four videos of space ships poking out of portals looking into outer space. Each video is in a grid formation. The top left video have both clipping and crossing mode disabled, so the space ship is being bounded by the portal geometry. The bottom left video have clipping mode set to plane and crossing mode disabled, so the space ship is clipped by the portal plane. The two videos on the right column have crossing mode enabled, so the spaceship is rendered outside the portal geometry. 

Play 

The spaceships below *don’t* have a PortalCrossingComponent.

 Video with custom controls. 

 Content description: Four videos of space ships poking out of portals looking into outer space. Each video is in a grid formation. The two videos on the top row have clipping mode disabled so the space ships are bounded by the portal geometry. The two videos on the bottom row have clipping mode enabled so the space ships are clipped by the portal plane. 

Play 

### Lighting

You define the lighting in a portal world with ImageBasedLightComponent and ImageBasedLightReceiverComponent.

RealityKit provides a default IBL if you don’t specify one with ImageBasedLightReceiverComponent.

Contents within a portal world don’t receive real-world probe lighting. However, you can achieve a similar effect in the portal world using VirtualEnvironmentProbeComponent.

You can configure this virtual probe lighting contribution with EnvironmentLightingConfigurationComponent.

Dynamic lights, such as PointLightComponent and DirectionalLightComponent, don’t cross world bounds.

Different lighting environments light the portal crossing entities based on which side of the portal they are on:

- When inside the portal, the portal world’s lighting lights the entity.

- When outside the portal, the default world’s lighting lights the entity.

## Topics

### Structures

struct ClippingPlane

A representation of a portal as an infinite plane.

struct Options

Options to toggle the portal features on and off.

struct Plane

A representation of a portal as an infinite plane.

### Initializers

init(target: Entity, clippingMode: PortalComponent.ClippingMode, crossingMode: PortalComponent.CrossingMode)

Creates a portal component with a target entity, clipping mode, and crossing mode.

init(target: Entity, clippingPlane: PortalComponent.ClippingPlane?)

Creates a portal component with a target entity and a clipping plane.

init(target: Entity, plane: PortalComponent.Plane, options: PortalComponent.Options)

Creates a portal component with a target entity, a single planar definition, and portal options.

### Instance Properties

var clippingMode: PortalComponent.ClippingMode

The clipping behavior of the portal component.

var clippingPlane: PortalComponent.ClippingPlane?

The clipping plane of the portal, using the entity’s local coordinates.

var crossingMode: PortalComponent.CrossingMode

The crossing behavior of the portal component.

var targetEntity: Entity?

The root entity for the portal’s target world.

### Enumerations

enum ClippingMode

Specifies the mode of clipping for a portal.

enum CrossingMode

Specifies the mode of crossing for a portal.

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

struct WorldComponent

A component that defines a portal world.

struct PortalCrossingComponent

A component that allows entities to cross portal boundaries.

