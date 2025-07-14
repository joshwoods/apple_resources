

- RealityKit
- PortalComponent
-  init(target:clippingPlane:) 

Initializer

# init(target:clippingPlane:)

Creates a portal component with a target entity and a clipping plane.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(
    target: Entity,
    clippingPlane: PortalComponent.ClippingPlane? = nil
)
```

## Parameters 

`target`  

A target world entity the portal is looking into.

`clippingPlane`  

A planar representation of a portal to enable the clipping feature. When `nil`, clippingMode is PortalComponent.ClippingMode.disabled.

## Discussion

This initializes the PortalComponent with the given target entity, and an optional clipping plane. The target entity needs a WorldComponent in its component set.

To render a portal, an entity needs a PortalComponent and a ModelComponent, using one or more PortalMaterial instances.

This initializer is equivalent to setting clippingMode with the same PortalComponent.Plane.

