

- ARKit
- ARWorldTrackingConfiguration
- ARWorldTrackingConfiguration.EnvironmentTexturing
-  ARWorldTrackingConfiguration.EnvironmentTexturing.manual 

Case

# ARWorldTrackingConfiguration.EnvironmentTexturing.manual

The framework generates environment textures only for probe anchors you explicitly add to the session.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
case manual
```

## Discussion

When you use this environmentTexturing option, you must manually choose when and where to generate environment map textures:

1.  Create an AREnvironmentProbeAnchor object with a `transform` indicating its position in the scene.

2.  Add the probe anchor to the session with the add(anchor:) method.

If you display AR content using ARSCNView, SceneKit automatically retrieves texture maps from probe anchors and uses them to light the scene. Otherwise, use a delegate method such as session(_:didUpdate:) to find out when the probe anchor’s texture has been updated and access the environmentTexture property.

