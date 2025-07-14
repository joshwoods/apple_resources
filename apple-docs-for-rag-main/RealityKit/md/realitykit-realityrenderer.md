

- RealityKit
-  RealityRenderer 

Class

# RealityRenderer

A renderer that displays a RealityKit scene in an existing Metal workflow.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
class RealityRenderer
```

## Overview

All RealityKit APIs for loading resources, creating entities and adding components are compatible and work with `RealityRenderer`.

## Topics

### Structures

struct CameraOutput

Output produced by rendering with a camera.

struct CameraSettings

Settings for rendering with a camera.

struct EntityCollection

A collection of entities in a RealityRenderer.

struct ImageBasedLight

Describe the lighting properties for the scene.

struct MetalEventAction

The structure describing an event and value to be signaled or waited for.

### Initializers

init() throws

### Instance Properties

var activeCamera: Entity?

The camera to be used for rendering.

var cameraSettings: RealityRenderer.CameraSettings

The settings to be used for rendering with `activeCamera`.

var entities: RealityRenderer.EntityCollection

A collection of RealityKit entities that this renderer renders within the scene.

var extendedDynamicRangeHeadroom: Float

var extendedDynamicRangeOutput: Bool

var lighting: RealityRenderer.ImageBasedLight

The lighting used in the environment of a particular scene.

### Instance Methods

func subscribe&lt;E>(to: E.Type, on: (any EventSource)?, componentType: (any Component.Type)?, (E) -> Void) -> EventSubscription

Subscribes to an event type, optionally limited to events affecting a source entity or scene, or limited to a specific component type for component events.

func update(TimeInterval) throws

Tick the simulation

func updateAndRender(deltaTime: TimeInterval, cameraOutput: RealityRenderer.CameraOutput, whenScheduled: ((RealityRenderer) -> Void)?, onComplete: ((RealityRenderer) -> Void)?, actionsBeforeRender: [RealityRenderer.MetalEventAction], actionsAfterRender: [RealityRenderer.MetalEventAction]) throws

Tick the simulation and render using activeCamera and the camera rendering output.

## See Also

### Metal workflow rendering

struct CameraSettings

Settings for rendering with a camera.

struct CameraOutput

Output produced by rendering with a camera.

struct ImageBasedLight

Describe the lighting properties for the scene.

struct MetalEventAction

The structure describing an event and value to be signaled or waited for.

struct EntityCollection

A collection of entities in a RealityRenderer.

