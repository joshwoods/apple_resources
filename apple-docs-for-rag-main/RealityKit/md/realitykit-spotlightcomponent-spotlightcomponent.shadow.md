

- RealityKit
- SpotLightComponent
-  SpotLightComponent.Shadow 

Structure

# SpotLightComponent.Shadow

A spotlight component that adds shadows to entities that it illuminates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
struct Shadow
```

## Topics

### Creating a shadow

init()

Creates a new spot light shadow object.

### Configuring the shadow

var depthBias: Float

A constant value that RealityKit applies as a bias to its shadow calculations.

var zNear: SpotLightComponent.Shadow.ShadowClippingPlane

The near-plane of a shadow frustum.

var zFar: SpotLightComponent.Shadow.ShadowClippingPlane

The orthogonal plane of the shadow frustum that’s furthest from the spotlight.

var cullModeOverride: SpotLightComponent.Shadow.ShadowMapCullMode?

The light’s culling mode for shadow map rendering.

### Registering a component type

static func registerComponent()

Registers a new component type.

### Comparing shadows

static func == (SpotLightComponent.Shadow, SpotLightComponent.Shadow) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Type Aliases

typealias ShadowMapCullMode

### Enumerations

enum ShadowClippingPlane

An object that specifies the mode of a shadow clipping plane.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Spotlights and their shadows

struct SpotLightComponent

A component that defines a spotlight source.

enum ShadowClippingPlane

An object that specifies the mode of a shadow clipping plane.

typealias ShadowMapCullMode

