

- RealityKit
- PortalComponent
-  init(target:clippingMode:crossingMode:) 

Initializer

# init(target:clippingMode:crossingMode:)

Creates a portal component with a target entity, clipping mode, and crossing mode.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    target: Entity,
    clippingMode: PortalComponent.ClippingMode,
    crossingMode: PortalComponent.CrossingMode
)
```

## Parameters 

`target`  

A target world entity the portal is looking into.

`clippingMode`  

A configuration for the portal’s clipping feature.

`crossingMode`  

A configuration for the portal’s crossing feature.

## Discussion

To render a portal, an entity needs a PortalComponent and a ModelComponent, using one or more PortalMaterial instances.

The target entity needs to have a WorldComponent or the portal does not render.

Provide PortalComponent.ClippingMode and PortalComponent.CrossingMode to configure the corresponding clipping and crossing features.

Using this initializer is equivalent to setting targetEntity, clippingMode and crossingMode properties directly.

See PortalComponent for example usage.

