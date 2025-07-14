

- RealityKit
-  RealityViewCameraContent 

Structure

# RealityViewCameraContent

The content of a reality view that is displayed through a camera.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct RealityViewCameraContent
```

## Overview

On iOS, `RealityViewCameraContent` displays content in an AR camera view by default, and can display in a “non-AR” mode when requested or when AR or the device’s camera is unavailable. On macOS, `RealityViewCameraContent` always displays its content in a non-AR mode.

You can use `RealityViewCameraContent` to add and remove entities, subscribe to RealityKit events, configure the AR environment, and perform coordinate conversions such as projections and raycasts between the RealityView space and a SwiftUI View coordinate space.

## Topics

### Structures

struct Body

The default view contents of a RealityView using RealityViewCameraContent.

### Instance Properties

var audioListener: Entity?

The entity which defines the listener position and orientation for spatial audio.

var camera: RealityViewCamera

The active camera for the RealityKit scene.

var cameraTarget: Entity?

The entity which an orbit camera targets.

var entities: RealityViewEntityCollection

A collection of RealityKit entities that this view content renders within the scene.

var environment: RealityViewEnvironment

The view’s background and default lighting properties.

var renderingEffects: RealityViewRenderingEffects

The rendering options that you use to selectively enable or disable certain rendering effects.

### Instance Methods

func subscribe&lt;E>(to: E.Type, on: (any EventSource)?, componentType: (any Component.Type)?, (E) -> Void) -> EventSubscription

Subscribes to an event type, optionally limited to events affecting a source entity or scene, or a specific component type for component events.

### Type Aliases

typealias Entities

The type of collection used for `entities`.

### Default Implementations

RealityCoordinateSpaceProjecting Implementations

RealityViewContentProtocol Implementations

## Relationships

### Conforms To

- Copyable
- RealityCoordinateSpaceProjecting
- RealityViewContentProtocol

## See Also

### SwiftUI scene presentation

struct RealityView

A view that contains RealityKit content.

struct RealityViewContent

The content of a visionOS reality view.

protocol RealityViewContentProtocol

A protocol representing the content of a reality view.

struct RealityViewDefaultPlaceholder

A view that represents the default placeholder for a RealityView.

struct RealityViewEntityCollection

A collection of entities in a RealityView.

protocol EntityCollection

An ordered, mutable collection of entities.

