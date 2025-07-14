

- RealityKit
-  SceneUnderstandingComponent 

Structure

# SceneUnderstandingComponent

A component that specifies an entity is participating in the system’s scene-understanding features.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+visionOS

``` source
struct SceneUnderstandingComponent
```

## Mentioned in 

Implementing scene understanding and reconstruction in your RealityKit app

## Overview

Scene understanding refers to RealityKit features like physics collision, shadows, and occlusion with real-world geometry. In iOS, `SceneUnderstandingComponent` is a read-only component. Manually adding it doesn’t have any effect.

In visionOS, `SceneUnderstandingComponent` is a write-only component. Add `SceneUnderstandingComponent` to your custom entities to let it behave as a virtual scene-understanding mesh.

For more information about scene-understanding features, see Implementing scene understanding and reconstruction in your RealityKit app.

## Topics

### Initializing a scene-understanding component

init()

Creates a component that makes an entity aware of certain aspects of the physical environment.

init(entityType: SceneUnderstandingComponent.EntityType?)

Creates a component for the given entity type that makes an entity aware of certain aspects of the physical environment.

### Managing the component

var entityType: SceneUnderstandingComponent.EntityType?

The type of real-world objects that the component models.

enum EntityType

Types of real-world objects that a scene-understanding component models.

static func registerComponent()

Registers a new component type.

### Instance Properties

var origin: SceneUnderstandingComponent.Origin

The origin that RealityKit creates the component from.

### Enumerations

enum Origin

Types of scene-understanding origins this component lives in.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Scene reconstructions and analysis

Creating a game with scene understanding

Create AR games and experiences that interact with real-world objects on LiDAR-equipped iOS devices.

Implementing scene understanding and reconstruction in your RealityKit app

Detect objects in an AR scene or create a detailed 3D reconstruction of the real-world environment.

Visualizing and interacting with a reconstructed scene

Estimate the shape of the physical environment using a polygonal mesh.

var sceneReconstruction: ARConfiguration.SceneReconstruction { get set }

A flag that enables scene reconstruction.

class func supportsSceneReconstruction(_ sceneReconstruction: ARConfiguration.SceneReconstruction) -> Bool

Checks if the device supports scene reconstruction.

struct SceneUnderstanding

An object that holds scene-understanding options for the view.

struct Options

Available scene-understanding options.

protocol HasSceneUnderstanding

A specification that detects and reacts to features of the physical environment.

final class SceneReconstructionProvider

A source of live data about the shape of a person’s surroundings.

class ARSession

The object that manages the major tasks associated with every AR experience, such as motion tracking, camera passthrough, and image analysis.

