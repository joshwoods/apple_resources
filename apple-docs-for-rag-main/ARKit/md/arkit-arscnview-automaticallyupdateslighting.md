

- ARKit
- ARSCNView
-  automaticallyUpdatesLighting 

Instance Property

# automaticallyUpdatesLighting

A Boolean value that specifies whether ARKit creates and updates SceneKit lights in the view’s scene.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@MainActor
var automaticallyUpdatesLighting: Bool { get set }
```

## Discussion

If this value is true (the default), the view automatically creates one or more SCNLight objects, adds them to the scene, and updates their properties to reflect estimated lighting information from the camera scene. Set this value to false if you want to directly control all lighting in the SceneKit scene.

