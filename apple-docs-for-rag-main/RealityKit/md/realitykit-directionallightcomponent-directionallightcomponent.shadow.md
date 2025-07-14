

- RealityKit
- DirectionalLightComponent
-  DirectionalLightComponent.Shadow 

Structure

# DirectionalLightComponent.Shadow

A directional light component that adds shadows to entities that it illuminates

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
struct Shadow
```

## Topics

### Creating the shadow

init()

Creates a directional light shadow using default values.

init(shadowProjection: DirectionalLightComponent.Shadow.ShadowProjectionType, depthBias: Float, cullMode: DirectionalLightComponent.Shadow.ShadowMapCullMode?)

Creates a directional light shadow with a shadow projection, depth bias and cull mode.

init(maximumDistance: Float, depthBias: Float)

Creates a directional light shadow with a maximum distance and depth bias.

### Configuring the shadow

var depthBias: Float

A constant value that RealityKit applies as a bias to its shadow calculations.

var cullModeOverride: DirectionalLightComponent.Shadow.ShadowMapCullMode?

The light’s culling mode for shadow map rendering.

var shadowProjection: DirectionalLightComponent.Shadow.ShadowProjectionType

Sets the shadow projection used for shadow map rendering

var maximumDistance: Float

The maximum distance for the shadow.

Deprecated

### Registering a component type

static func registerComponent()

Registers a new component type.

### Comparing shadows

static func == (DirectionalLightComponent.Shadow, DirectionalLightComponent.Shadow) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Type Aliases

typealias ShadowMapCullMode

### Enumerations

enum ShadowProjectionType

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Directional lights and their shadows

struct DirectionalLightComponent

A component that defines a directional light source.

enum ShadowProjectionType

typealias ShadowMapCullMode

