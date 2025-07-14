

- RealityKit
-  Scenes 

API Collection

# Scenes

The context that holds all RealityKit entities.

## Overview

The system adds an Entity to a Scene when you add it to a RealityView with a RealityViewCameraContent or RealityViewContent instance. These scenes contain anchors and a hierarchy of entities that make up your RealityKit content.

The Scene instance has helpful methods to perform ray casts to help you better understand your scene, and methods that find entities either by name or by components they own.

## Topics

### Scene management

class Scene

A container that holds the collection of entities that an AR view renders.

struct AnchorCollection

A collection of anchor entities.

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Entity searches

struct QueryPredicate

An object that defines the criteria for an entity query.

struct PixelCastHit

### Event publishers and subscription

enum SceneEvents

Events the scene invokes.

struct Publisher

A publisher for the given event type in the scene.

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

struct SceneUnderstandingComponent

A component that specifies an entity is participating in the system’s scene-understanding features.

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

## See Also

### Scene management and logic

Systems

Apply behaviors and physical effects to the entities in a RealityKit scene.

Events

Respond to things happening in your RealityKit scene by subscribing to specific event types.

Entity actions

Create simple, reusable actions that can change your app state, RealityKit scene, or animate an entity.

