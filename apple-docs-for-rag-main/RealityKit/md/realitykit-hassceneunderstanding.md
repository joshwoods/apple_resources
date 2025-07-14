

- RealityKit
-  HasSceneUnderstanding 

Protocol

# HasSceneUnderstanding

A specification that detects and reacts to features of the physical environment.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+visionOS

``` source
@MainActor @preconcurrency
protocol HasSceneUnderstanding : Entity
```

## Topics

### Understanding the scene

var sceneUnderstanding: SceneUnderstandingComponent

An entity component that detects and reacts to features of the physical environment.

## Relationships

### Inherits From

- Entity

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

struct SceneUnderstandingComponent

A component that specifies an entity is participating in the system’s scene-understanding features.

struct SceneUnderstanding

An object that holds scene-understanding options for the view.

struct Options

Available scene-understanding options.

final class SceneReconstructionProvider

A source of live data about the shape of a person’s surroundings.

class ARSession

The object that manages the major tasks associated with every AR experience, such as motion tracking, camera passthrough, and image analysis.

