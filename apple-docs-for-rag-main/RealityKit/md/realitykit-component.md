

- RealityKit
-  Component 

Protocol

# Component

A representation of a geometry or a behavior that you apply to an entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
protocol Component
```

## Overview

You assemble a particular combination of behavior and appearance for an entity by adding components to the components set of an Entity instance. Each component, represented by a type that conforms to the Component protocol, defines a single aspect of the entity. For example, one might define a position in space, while another provides a visual appearance. You can add at most one component of a given type to an entity.

RealityKit has a variety of predefined component types that you can use to add commonly needed characteristics. For example, the ModelComponent specifies visual appearance with a mesh and materials. The CollisionComponent contains a shape and other information used to decide if one entity collides with another.

You can also define custom component types. When you do, register that type with the system by calling the new component’s registerComponent() method—a default implementation of which is provided by the Component protocol. Call this method once before using the component type. You don’t need to make this call for component types that RealityKit provides.

Tip

You can subscribe to ComponentEvents for events that the system triggers when you interact with components.

## Topics

### Registering a component type

static func registerComponent()

Registers a new component type.

## Relationships

### Inherited By

- TransientComponent

### Conforming Types

- AccessibilityComponent
- AdaptiveResolutionComponent
- AmbientAudioComponent
- AnchoringComponent
- AnimationLibraryComponent
- AudioLibraryComponent
- AudioMixGroupsComponent
- BillboardComponent
- BlendShapeWeightsComponent
- BodyTrackingComponent
- ChannelAudioComponent
- CharacterControllerComponent
- CharacterControllerStateComponent
- CollisionComponent
- DirectionalLightComponent
- DirectionalLightComponent.Shadow
- DockingRegionComponent
- DynamicLightShadowComponent
- EnvironmentLightingConfigurationComponent
- ForceEffectComponent
- GeometricPinsComponent
- GroundingShadowComponent
- HoverEffectComponent
- IKComponent
- ImageBasedLightComponent
- ImageBasedLightReceiverComponent
- InputTargetComponent
- ModelComponent
- ModelDebugOptionsComponent
- ModelSortGroupComponent
- OpacityComponent
- OrthographicCameraComponent
- ParticleEmitterComponent
- PerspectiveCameraComponent
- PhysicsBodyComponent
- PhysicsJointsComponent
- PhysicsMotionComponent
- PhysicsSimulationComponent
- PointLightComponent
- PortalComponent
- PortalCrossingComponent
- ProjectiveTransformCameraComponent
- ReferenceComponent
- ReverbComponent
- SceneUnderstandingComponent
- SkeletalPosesComponent
- SpatialAudioComponent
- SpotLightComponent
- SpotLightComponent.Shadow
- SynchronizationComponent
- TextComponent
- Transform
- VideoPlayerComponent
- ViewAttachmentComponent
- VirtualEnvironmentProbeComponent
- WorldComponent

## See Also

### Essentials

Understanding the modular architecture of RealityKit

Learn how everything fits together in RealityKit.

Building an immersive experience with RealityKit

Use systems and postprocessing effects to create a realistic underwater scene.

class Entity

An element of a RealityKit scene to which you attach components that provide appearance and behavior characteristics for the entity.

