

- ARKit
- ARSCNView
-  scene 

Instance Property

# scene

The SceneKit scene to be displayed in the view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@MainActor
var scene: SCNScene { get set }
```

## Discussion

Note

Unlike the parent SCNView class, an ARSCNView object requires a non-`nil` scene to display.

## See Also

### Essentials

Providing 3D Virtual Content with SceneKit

Use SceneKit to add realistic three-dimensional objects to your AR experience.

var session: ARSession

The AR session that manages motion tracking and camera image processing for the view’s contents.

