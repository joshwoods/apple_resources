

- RealityKit
- SpotLightComponent
- SpotLightComponent.Shadow
-  SpotLightComponent.Shadow.ShadowClippingPlane 

Enumeration

# SpotLightComponent.Shadow.ShadowClippingPlane

An object that specifies the mode of a shadow clipping plane.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum ShadowClippingPlane
```

## Topics

### Clipping plane options

case automatic

The spotlight component automatically sets the position of the shadow clipping plane.

case fixed(Float)

The shadow clipping plane’s position doesn’t change.

### Comparing shadow clipping planes

static func == (SpotLightComponent.Shadow.ShadowClippingPlane, SpotLightComponent.Shadow.ShadowClippingPlane) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Spotlights and their shadows

struct SpotLightComponent

A component that defines a spotlight source.

struct Shadow

A spotlight component that adds shadows to entities that it illuminates.

typealias ShadowMapCullMode

