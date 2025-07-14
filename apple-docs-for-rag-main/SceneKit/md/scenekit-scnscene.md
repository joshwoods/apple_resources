

- SceneKit
-  SCNScene 

Class

# SCNScene

A container for the node hierarchy and global properties that together form a displayable 3D scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNScene
```

## Overview

To display 3D content with SceneKit, you create a scene containing a hierarchy of the nodes and attributes that together represent your visual elements. Typically, you build your assets in a 3D visual editor, then assemble them into a scene using Xcode’s SceneKit Scene Editor, ready for SceneKit to render.

To display your scene, you need to load it at runtime, then set it as the scene property of an SCNView:

```
guard let myScene = SCNScene(named: "MyScene") 
    else { fatalError("Unable to load scene file.") }
scnView.scene = myScene // Your app's SCNView
```

### Creating a Scene

The simplest way to create a scene is through Xcode’s SceneKit Scene Editor. Start by importing one or more assets from a 3D editor, such as Blender. Then you adjust the positions and attributes of the assets, and set global scene properties, such as lighting environment, to compose your scene. The scene editor creates a `.scn` file, which you save to a `.scnassets` folder in the app bundle. When you build your project, Xcode optimizes the scene file for your target platform.

## Topics

### Creating a Scene from a File

convenience init?(named: String)

Loads a scene from a file with the specified name in the app’s main bundle.

convenience init?(named: String, inDirectory: String?, options: [SCNSceneSource.LoadingOption : Any]?)

Loads a scene from a file with the specified name in a specific subdirectory of the app’s main bundle.

convenience init(url: URL, options: [SCNSceneSource.LoadingOption : Any]?) throws

Loads a scene from the specified URL.

### Managing Animated Effects in a Scene

var isPaused: Bool

A Boolean value that determines whether to run actions, animations, particle systems, and physics simulations in the scene graph.

### Accessing Scene Contents

var rootNode: SCNNode

The root node of the scene graph.

var background: SCNMaterialProperty

A background to be rendered before the rest of the scene.

var lightingEnvironment: SCNMaterialProperty

A cube map texture that depicts the environment surrounding the scene’s contents, used for advanced lighting effects.

### Managing Scene Attributes

func attribute(forKey: String) -> Any?

Returns the scene attribute for the specified key.

func setAttribute(Any?, forKey: String)

Sets a scene attribute for the specified key.

struct Attribute

### Exporting a Scene File

func write(to: URL, options: [String : Any]?, delegate: (any SCNSceneExportDelegate)?, progressHandler: SCNSceneExportProgressHandler?) -> Bool

Exports the scene and its contents to a file at the specified URL.

protocol SCNSceneExportDelegate

Methods you can implement to participate in the process of exporting a scene to a file.

### Adding Fog to a Scene

var fogStartDistance: CGFloat

The distance from a point of view at which the scene’s contents begin to be obscured by fog. Animatable.

var fogEndDistance: CGFloat

The distance from a point of view at which the scene’s contents are completely obscured by fog. Animatable.

var fogDensityExponent: CGFloat

The transition curve for the fog’s intensity between its start and end distances. Animatable.

var fogColor: Any

The color of the fog effect to be rendered with the scene. Animatable.

### Working With Physics in the Scene

var physicsWorld: SCNPhysicsWorld

The physics simulation associated with the scene.

### Working with Particle Systems in the Scene

func addParticleSystem(SCNParticleSystem, transform: SCNMatrix4)

Attaches a particle system to the scene, using the specified transform.

var particleSystems: [SCNParticleSystem]?

The particle systems attached to the scene.

func removeParticleSystem(SCNParticleSystem)

Removes a particle system attached to the scene.

func removeAllParticleSystems()

Removes any particle systems directly attached to the scene.

### Constants

Scene Attributes

Attribute keys available in the options dictionary for the methods attribute(forKey:) and setAttribute(_:forKey:)

Scene Export Options

Options for the write(to:options:delegate:progressHandler:) method.

typealias SCNSceneExportProgressHandler

The signature for the block that SceneKit calls during scene export.

### Instance Properties

var screenSpaceReflectionMaximumDistance: CGFloat

var screenSpaceReflectionSampleCount: Int

var screenSpaceReflectionStride: CGFloat

var wantsScreenSpaceReflection: Bool

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GKSceneRootNodeType
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Essentials

class SCNView

A view for displaying 3D SceneKit content.

