

- ARKit
- ARKit in iOS
- Camera, Lighting, and Effects
-  Visualizing and interacting with a reconstructed scene 

Sample Code

# Visualizing and interacting with a reconstructed scene

Estimate the shape of the physical environment using a polygonal mesh.

Download

iOS 13.4+iPadOS 13.4+Xcode 16.0+

## Overview

On a fourth-generation iPad Pro running iPad OS 13.4 or later, ARKit uses the LiDAR Scanner to create a polygonal model of the physical environment. The LiDAR Scanner quickly retrieves depth information from a wide area in front of the user, so ARKit can estimate the shape of the real world without requiring the user to move. ARKit converts the depth information into a series of vertices that connect to form a *mesh*. To partition the information, ARKit makes multiple anchors, each assigned a unique portion of the mesh. Collectively, the mesh anchors represent the real-world *scene* around the user.

With these meshes, you can:

- More accurately locate points on real-world surfaces.

- Classify real-world objects that ARKit can recognize.

- Occlude your app’s virtual content with real-world objects that are in front of it.

- Have virtual content interact with the physical environment realistically, for example, by bouncing a virtual ball off a real-world wall and having the ball follow the laws of physics.

This sample app presents an AR experience using RealityKit. The figure below illustrates how RealityKit leverages real-world information from ARKit, and creates a debug visualization when you run this app and point the device at a real-world chair.

## Visualize the shape of the physical environment

To enable scene meshes, the sample sets a world-configuration’s sceneReconstruction property to one of the mesh options.

```
arView.automaticallyConfigureSession = false
let configuration = ARWorldTrackingConfiguration()
configuration.sceneReconstruction = .meshWithClassification
```

The sample uses RealityKit’s ARView to render its graphics. To visualize meshes at runtime, ARView offers the sceneUnderstanding debugging option.

```
arView.debugOptions.insert(.showSceneUnderstanding)
```

Note

The sample enables mesh visualization only to demonstrate the mesh feature; similarly, you normally enable mesh visualization only for debugging purposes.

To begin the AR experience, the sample configures and runs the session when the app first starts, in the main view controller’s `viewDidLoad` callback.

```
arView.session.run(configuration)
```

### Add plane detection

When an app enables plane detection with scene reconstruction, ARKit considers that information when making the mesh. Where the LiDAR scanner may produce a slightly uneven mesh on a real-world surface, ARKit smooths out the mesh where it detects a plane on that surface.

To demonstrate the difference that plane detection makes on meshes, this app displays a toggle button. In the button handler, the sample adjusts the plane-detection configuration and restarts the session to effect the change.

```
@IBAction func togglePlaneDetectionButtonPressed(_ button: UIButton) {
    guard let configuration = arView.session.configuration as? ARWorldTrackingConfiguration else {
        return
    }
    if configuration.planeDetection == [] {
        configuration.planeDetection = [.horizontal, .vertical]
        button.setTitle("Stop Plane Detection", for: [])
    } else {
        configuration.planeDetection = []
        button.setTitle("Start Plane Detection", for: [])
    }
    arView.session.run(configuration)
}
```

## Locate a Point on an Object’s Surface

Apps that retrieve surface locations using meshes can achieve unprecedented accuracy. By considering the mesh, raycasts can intersect with nonplanar surfaces, or surfaces with little or no features, like white walls.

To demonstrate accurate raycast results, this app casts a ray when the user taps the screen. The sample specifies the ARRaycastQuery.Target.estimatedPlane allowable-target, and ARRaycastQuery.TargetAlignment.any alignment option, as required to retrieve a point on a meshed, real-world object.

```
if let result = arView.raycast(from: tapLocation, allowing: .estimatedPlane, alignment: .any).first {
    // ...
```

When the user’s raycast returns a result, this app gives visual feedback by placing a small sphere at the intersection point.

```
let resultAnchor = AnchorEntity(world: result.worldTransform)
resultAnchor.addChild(sphere(radius: 0.01, color: .lightGray))
arView.scene.addAnchor(resultAnchor, removeAfter: 3)
```

## Classify Real-World Objects

ARKit has a classification feature that analyzes its meshed model of the world to recognize specific, real-world objects. Within the mesh, ARKit can classify floors, tables, seats, windows, and ceilings. See ARMeshClassification for the full list.

If the user taps the screen and the raycast intersects with a meshed, real-world object, this app displays text of the mesh’s classification.

When the automaticallyConfigureSession property of ARView is `true`, RealityKit disables classification by default because it isn’t required for occlusion and physics. To enable mesh classification, the sample overrides the default by setting the sceneReconstruction property to meshWithClassification.

```
arView.automaticallyConfigureSession = false
let configuration = ARWorldTrackingConfiguration()
configuration.sceneReconstruction = .meshWithClassification
```

This app attempts to retrieve a classification for the intersection point from the mesh.

```
nearbyFaceWithClassification(to: result.worldTransform.position) { (centerOfFace, classification) in
    // ...
```

Every three vertices in the mesh form a triangle, called a *face.* ARKit assigns a classification for each face, so the sample searches through the mesh for a face near the intersection point. If the face has a classification, this app displays it on screen. Because this routine involves extensive processing, the sample does the work asynchronously, so the renderer does not stall.

```
DispatchQueue.global().async {
    for anchor in meshAnchors {
        for index in 0..(geometricCenterOfFace.0, geometricCenterOfFace.1, geometricCenterOfFace.2, 1)
            let centerWorldPosition = (anchor.transform * centerLocalTransform).position

            // We're interested in a classification that is sufficiently close to the given location––within 5 cm.
            let distanceToFace = distance(centerWorldPosition, location)
            if distanceToFace 

With the classification in-hand, the sample creates 3D text to display it.

```
let textEntity = self.model(for: classification)
```

To prevent the mesh from partially occluding the text, the sample offsets the text slightly to help readability. The sample calculates the offset in the negative direction of the ray, which effectively moves the text slightly toward the camera, which is away from the surface.

```
let rayDirection = normalize(result.worldTransform.position - self.arView.cameraTransform.translation)
let textPositionInWorldCoordinates = result.worldTransform.position - (rayDirection * 0.1)
```

To make the text always appear the same size on screen, the sample applies a scale based on text’s distance from the camera.

```
let raycastDistance = distance(result.worldTransform.position, self.arView.cameraTransform.translation)
textEntity.scale = .one * raycastDistance
```

To display the text, the sample puts it in an anchored entity at the adjusted intersection-point, which is oriented to face the camera.

```
var resultWithCameraOrientation = self.arView.cameraTransform
resultWithCameraOrientation.translation = textPositionInWorldCoordinates
let textAnchor = AnchorEntity(world: resultWithCameraOrientation.matrix)
textAnchor.addChild(textEntity)
self.arView.scene.addAnchor(textAnchor, removeAfter: 3)
```

To visualize the location of the face’s vertex from which the classification was retrieved, the sample creates a small sphere at the vertex’s real-world position.

```
if let centerOfFace = centerOfFace {
    let faceAnchor = AnchorEntity(world: centerOfFace)
    faceAnchor.addChild(self.sphere(radius: 0.01, color: classification.color))
    self.arView.scene.addAnchor(faceAnchor, removeAfter: 3)
    // ...
}
```

### Occlude virtual content with a mesh

*Occlusion* is a feature where parts of the real world cover an app’s virtual content, from the camera’s perspective. To achieve this illusion, RealityKit checks for any meshes in front of virtual content, viewed by the user, and omits drawing any part of the virtual content obscured by those meshes. The sample enables occlusion by adding the ARView.Environment.SceneUnderstanding.Options option to the environment’s sceneUnderstanding property.

```
arView.environment.sceneUnderstanding.options.insert(.occlusion)
```

At runtime, this app omits drawing portions of the virtual text that are behind any part of the meshed, real world.

### Interact with real-world objects using physics

With scene meshes, virtual content can interact with the physical environment realistically because the meshes give RealityKit’s physics engine an accurate model of the world. The sample enables physics by adding the physics option to the environment’s sceneUnderstanding property.

```
arView.environment.sceneUnderstanding.options.insert(.physics)
```

To detect when virtual content comes in contact with a meshed, real-world object, the sample defines the text’s proportions using a collision shape in the `addAnchor(_:,removeAfter:)` scene extension.

```
if model.collision == nil {
    model.generateCollisionShapes(recursive: true)
    model.physicsBody = .init()
}
```

When this app classifies an object and displays some text, it waits three seconds before dropping the virtual text. When the sample sets the text’s physicsBody’s mode to PhysicsBodyMode.dynamic, the text reacts to gravity by falling.

```
Timer.scheduledTimer(withTimeInterval: seconds, repeats: false) { (timer) in
    model.physicsBody?.mode = .dynamic
}
```

As the text falls, it reacts when colliding with a meshed, real-world object, such as landing on the floor.

## See Also

### Occlusion

Occluding virtual content with people

Cover your app’s virtual content with people that ARKit perceives in the camera feed.

Effecting People Occlusion in Custom Renderers

Occlude your app’s virtual content where ARKit recognizes people in the camera feed by using matte generator.

class ARMatteGenerator

An object that creates matte textures you use to occlude your app’s virtual content with people, that ARKit recognizes in the camera feed.

