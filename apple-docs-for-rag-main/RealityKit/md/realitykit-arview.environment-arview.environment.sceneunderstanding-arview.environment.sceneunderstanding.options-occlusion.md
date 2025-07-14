

- RealityKit
- ARView
- 
  - ARView
- ARView.Environment
- ARView.Environment.SceneUnderstanding
- ARView.Environment.SceneUnderstanding.Options
-  occlusion 

Type Property

# occlusion

The `.occlusion` option means that the reconstructed geometry will be used for rendering, but only to update the depth buffer. Parts of virtual objects which are behind the reconstructed geometry are not rendered.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15+

``` source
static let occlusion: ARView.Environment.SceneUnderstanding.Options
```

