

- RealityKit
- ARView
-  scene 

Instance Property

# scene

The scene that the view renders and simulates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
@MainActor @preconcurrency
var scene: Scene { get }
```

## Discussion

When you initialize a view, it comes with a single Scene instance that you access through the view’s scene property. Add AnchorEntity instances to the scene’s anchors collection to provide content for the scene.

