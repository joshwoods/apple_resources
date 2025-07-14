

- RealityKit
- ARView
- ARView.Environment
- ARView.Environment.SceneUnderstanding
-  ARView.Environment.SceneUnderstanding.Options 

Structure

# ARView.Environment.SceneUnderstanding.Options

Available scene-understanding options.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15+

``` source
struct Options
```

## Topics

### Initializers

init(rawValue: UInt32)

Creates a new option set from the given raw value.

### Instance Properties

let rawValue: UInt32

The corresponding value of the raw type.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let collision: ARView.Environment.SceneUnderstanding.Options

The `.collision` option means that the reconstructed geometry can be used for collision queries (i.e. raycasting)

static let `default`: ARView.Environment.SceneUnderstanding.Options

The `.default` options is a sentinel value that indicates the user wants whatever scene-understanding features work with the current device and are supported. It overrides other options in the options set.

static let occlusion: ARView.Environment.SceneUnderstanding.Options

The `.occlusion` option means that the reconstructed geometry will be used for rendering, but only to update the depth buffer. Parts of virtual objects which are behind the reconstructed geometry are not rendered.

static let physics: ARView.Environment.SceneUnderstanding.Options

No abstract

static let receivesLighting: ARView.Environment.SceneUnderstanding.Options

The `.receivesLighting` option means that the virtual lights will interact with real world surfaces causing them to shine. The properties of the mesh will be set to a default material.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

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

protocol HasSceneUnderstanding

A specification that detects and reacts to features of the physical environment.

final class SceneReconstructionProvider

A source of live data about the shape of a person’s surroundings.

class ARSession

The object that manages the major tasks associated with every AR experience, such as motion tracking, camera passthrough, and image analysis.

