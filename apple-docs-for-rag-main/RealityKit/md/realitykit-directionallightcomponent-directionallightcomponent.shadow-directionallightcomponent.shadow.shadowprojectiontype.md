

- RealityKit
- DirectionalLightComponent
- DirectionalLightComponent.Shadow
-  DirectionalLightComponent.Shadow.ShadowProjectionType 

Enumeration

# DirectionalLightComponent.Shadow.ShadowProjectionType

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum ShadowProjectionType
```

## Topics

### Shadow projection types

case automatic(maximumDistance: Float)

Shadow projection is automatically fit with the camera frustum, range is within maximumDistance from camera

case fixed(zNear: Float, zFar: Float, orthographicScale: Float)

Shadow projection is manually set up with near plane, far plane, and orthographicScale for width and height

### Comparing shadow projection types

static func == (DirectionalLightComponent.Shadow.ShadowProjectionType, DirectionalLightComponent.Shadow.ShadowProjectionType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Directional lights and their shadows

struct DirectionalLightComponent

A component that defines a directional light source.

struct Shadow

A directional light component that adds shadows to entities that it illuminates

typealias ShadowMapCullMode

