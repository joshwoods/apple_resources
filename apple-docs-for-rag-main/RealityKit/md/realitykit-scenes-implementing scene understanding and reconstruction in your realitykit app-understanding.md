

- RealityKit
- Scenes
-  Implementing scene understanding and reconstruction in your RealityKit app 

Article

# Implementing scene understanding and reconstruction in your RealityKit app

Detect objects in an AR scene or create a detailed 3D reconstruction of the real-world environment.

## Overview

RealityKit can detect planes in the real-world environment on any device, allowing you to place virtual objects in the world and have them interact. On devices with a LiDAR sensor, RealityKit can create a detailed reconstruction of the surrounding environment, allowing more precise interactions between virtual content and the real world. With scene understanding enabled, RealityKit not only reconstructs the environment, but can also recognize what many real-world objects are.

### Use scene understanding in iOS and macOS

To enable scene-understanding in an iOS or macOS RealityKit app, insert options into sceneUnderstanding like this:

```
arView.environment.sceneUnderstanding.options.insert(.occlusion)
arView.environment.sceneUnderstanding.options.insert(.physics)
arView.environment.sceneUnderstanding.options.insert(.collision)
arView.environment.sceneUnderstanding.options.insert(.receivesLighting)
```

Or, if you’re using RealityView, you can configure the same options using SpatialTrackingSession.Configuration.

```
let session = SpatialTrackingSession()
let config = SpatialTrackingSession.Configuration(
    tracking:[],
    sceneUnderstanding:[
        .occlusion,
        .physics,
        .collision,
        .shadow
])
await session.run(config)
```

### Use scene reconstruction in iOS and macOS

After turning on scene-understanding options, RealityKit automatically generates entities representing real-world geometry with a SceneUnderstandingComponent.

You can get these entities by using an EntityQuery. Here’s an example of rendering a custom debug material with scene-understanding meshes:

```
var debugMaterial = UnlitMaterial(color: .green)
debugMaterial.triangleFillMode = .lines

let sceneUnderstandingQuery = EntityQuery(where: .has(SceneUnderstandingComponent.self) && .has(ModelComponent.self))
let queryResult = scene.performQuery(sceneUnderstandingQuery)
queryResult.forEach { entity in
    entity.components[ModelComponent.self]?.materials = [debugMaterial]
}
```

With physics or collision, scene-understanding meshes can participate in physics simulations and collision events.

Here’s an example of identifying scene-understanding meshes in a collision event:

```
let _ = content.subscribe(to: CollisionEvents.Began.self) { event in
    if event.entityA.components.has(SceneUnderstandingComponent.self) {
        // The entityA is a scene-understanding mesh.
    }
}
```

### Use scene understanding in visionOS

RealityKit doesn’t automatically provide scene-understanding meshes in visionOS. Instead, you can manually add SceneUnderstandingComponent to your custom entities to let it behave as a virtual scene-understanding mesh. A virtual scene-understanding mesh participates in system rendering features, such as shadows and depth mitigation, just like real-world geometry.

Custom virtual scene-understanding meshes only work in progressive or full immersive space. They don’t work in mixed space, or in a window or volume in the Shared Space.

### Use scene reconstruction in visionOS

To enable scene reconstruction for a visionOS app, use a SceneReconstructionProvider.

```
let arSession = ARKitSession()
let sceneReconstruction = SceneReconstructionProvider(modes: [])

Task {
    do {
        try await arSession.run([sceneReconstruction])
    } catch {
        // Handle the error.
    }
}
```

## See Also

### Scene reconstructions and analysis

Creating a game with scene understanding

Create AR games and experiences that interact with real-world objects on LiDAR-equipped iOS devices.

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

