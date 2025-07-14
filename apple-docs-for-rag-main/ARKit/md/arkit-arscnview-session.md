

- ARKit
- ARSCNView
-  session 

Instance Property

# session

The AR session that manages motion tracking and camera image processing for the view’s contents.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@MainActor
var session: ARSession { get set }
```

## Discussion

A view creates its own session object; use this property to access and configure the view’s session.

## See Also

### Essentials

Providing 3D Virtual Content with SceneKit

Use SceneKit to add realistic three-dimensional objects to your AR experience.

var scene: SCNScene

The SceneKit scene to be displayed in the view.

