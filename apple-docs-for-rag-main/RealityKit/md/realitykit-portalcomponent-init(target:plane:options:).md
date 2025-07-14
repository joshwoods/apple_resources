

- RealityKit
- PortalComponent
-  init(target:plane:options:) 

Initializer

# init(target:plane:options:)

Creates a portal component with a target entity, a single planar definition, and portal options.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    target: Entity,
    plane: PortalComponent.Plane,
    options: PortalComponent.Options
)
```

## Parameters 

`target`  

A target world entity the portal is looking into.

`plane`  

A plane for configuring clipping and crossing features.

`options`  

An option set that determines which clipping and crossing features to enable.

## Discussion

Use this initializer to toggle clippingMode and crossingMode with the same PortalComponent.Plane.

